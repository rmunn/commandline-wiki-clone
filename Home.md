Version 2 is currently released as [![NuGet](https://img.shields.io/nuget/v/CommandLineParser.svg)](https://nuget.org/packages/CommandLineParser)

```
PM> Install-Package CommandLineParser
```

# Overview
The package has no dependencies. The standard `CommandLineParser` package does not include references/dependencies for FSharp. Users that want support for F# should target the `CommandLineParser.FSharp` package.

# Getting Started
The Parser is activated from the `Parser` class, defined in the `CommandLine` namespace. I suggest that you use the pre-configured `Default` singleton, and only construct your own instance when really required.

```csharp
using CommandLine;

// (1) default singleton
var result = Parser.Default.ParseArguments<Options>(args);

// (2) build and configure instance
var parser = new Parser(with => with.EnableDashDash = true);
var result = parser.ParseArguments<Options>(args);
```

In the latter case the `Parser(Action<ParserSettings>)` constructor was called to configure the parser via the `ParserSettings` instance.

The `CommandLine.Text` namespace contains everything you need to create a user friendly help screen. This is done automatically if `ParserSettings.HelpWriter` is set.

The default instance `Parser.Default` initializes with `ParserSettings.HelpWriter` set to `Console.Error`.

These features are optional.
 
# Parsed Options and Value
Version 2 uses only two attributes to describe option syntax: `Option` and `Value`·

`Option` works much like in previous versions, but it can be applied to scalar or sequence values (`IEnumerable<T>`).

When applied to sequences you can also define `Min` and `Max` properties to specify a range of values.

`Value` resembles `ValueOption` and `ValueList` from previous versions. Akin to the new `Option` attribute, it can be applied to sequences, and now support the `Required` property too.

## [Value] Attribute

Values are partitioned by index. For example:
```csharp
class Options {
  [Value(0)]
  public int IntValue { get; set; }

  [Value(1, Min=1, Max=3)]
  public IEnumerable<string> StringSeq { get; set; }

  [Value(2)]
  public double DoubleValue { get; set; }
}
```

So long as you supply values, they will be set to corresponding properties:
```bash
$ app 10 str1 str2 str3 1.1
```

If you omit `Min` and `Max` constraints, all available values will be captured by the sequence. There's no point defining a `Value` attribute with a higher index than that of a sequence `Value` which lacks a **Max** range constraint:
```csharp
class Options {
  [Value(0)]
  public int IntValue { get; set; }

  [Value(1)]
  public IEnumerable<string> StringSeq { get; set; }

  // all values captured by previous specifications,
  // this property will never receive a value
  [Value(2)]
  public DoubleValue { get; set; }
}
```

## [Option] Attribute

If you Omit the option name the long name will be inferred from the member's name.
```csharp
class Options {
  [Option]
  public string UserId { get; set; }
}
```
This allows:
```bash
$ app --userid=root
```

`Option` attribute also supports a `Separator` property to mimic the deprecated `OptionList` behavior when applied to sequences.
```csharp
class Options {
  [Option('t', Separator=':')]
  public IEnumerable<string> Types { get; set; }
}
```
This allows:
```bash
$ app -t int:long:string
```

## Capturing Sequences

As mentioned above, you can apply both new attributes to `IEnumerable<T>` (where `T` is a CLR built-in data type such as `string`, `int`, etc).

You can also specify a `Min` constraint or a `Max` constraint alone: this means you only want check for minimum or maximum number of elements. Breaking a constraint will cause parsing to fail.

You could overlay `Min=1` with `Required=true` but there's no point in doing so because the parser will check `Required` before the `Min` constraint. In this case you should favour `Min=1` whilst `Min=1, Max=1` should be avoided (even though they will behave as expected) in favour of `Required=true`. 

# Parsing

Parsing is a single liner:
```csharp
var result = Parser.Default.ParseArguments<Options>(args);
```

The above is a basic usage scenario (without verbs) utilizing the default pre-built instance to parse input arguments using the rules specified in the `Options` class.

The `result` variable (defined here using implicit typing) is of type `ParserResult<T>`, where T is the options class you defined (e.g `ParserResult<Options>`).

If **parsing succeeds**, you'll get a derived `Parsed<T>` type that exposes an instance of `T` through its `Value` property.

If **parsing fails**, you'll get a derived `NotParsed<T>` type with errors present in `Errors` sequence.

Even though it's possible to examine the `Errors` sequence, it's recommended to quit with an appropriate error code. The library **help subsystem** will print out usage and error descriptions automatically. The parser default instance is configured to output this text to `Console.Error`. If the parser is instantiated by using the constructor, the `ParserSettings.HelpWriter` needs to be set properly in order for the help text to be shown. Refer to Section [Help Screen](#help-screen) for more detail.

This hierarchy is modeled like an **F#** discriminated union. You can check the property `Tag` to see which derived type you received, no need for casting.

Two convenient extension methods are provided to help you access values:
```csharp
var result = Parser.Default.ParseArguments<Options>(args)
  .WithParsed(options => ...) // options is an instance of Options type
  .WithNotParsed(errors => ...) // errors is a sequence of type IEnumerable<Error>
```

These methods accept a `System.Action` lambda, but if you prefer another approach, you can transform the parser result into any other value using `MapResult(...)` (and its overloads):
```csharp
// you can directly turn the result into an exit code for example
int Main(string[] args) {
  return Parser.Default.ParseArguments<Options>(args)
    .MapResult(
      options => RunAndReturnExitCode(options),
      _ => 1);
}
```

## Verbs

Verbs help delineate and separate options and values for multiple commands within a single app.  A common usage of verbs in a sample ftp program could be to provide a specific commands: upload, download, delete, etc.

To use verb commands create an option class for each verb decorated with the `[Verb]` attribute:
```csharp
[Verb("add", HelpText = "Add file contents to the index.")]
class AddOptions { //normal options here
}
[Verb("commit", HelpText = "Record changes to the repository.")]
class CommitOptions { //normal options here
}
[Verb("clone", HelpText = "Clone a repository into a new directory.")]
class CloneOptions { //normal options here
}
```

A this point you have to use a proper `ParserArguments<T1, T2...>` overload that accepts more than one type (without using the overload with variadic arguments, the library defines versions with up to 16 type parameters):
```csharp
var result = Parser.Default.ParseArguments<AddOptions, CommitOptions, CloneOptions>(args);
```

In this case the `T Value` property of `ParserResult<T>` will be `object` but will contain the proper instance if parsing succeeds or `NullInstance` if fails.

The only change with normal parsing is the requirement to query the `Parsed<object>.Value` property and invoke the application logic written to handle a specific verb.

A helper extension method is provided to simplify this task:
```csharp
Parser.Default.ParseArguments<AddOptions, CommitOptions, CloneOptions>(args)
  .WithParsed<AddOptions>(opts => ...)
  .WithParsed<CommitOptions>(opts => ...)
  .WithParsed<CloneOptions>(opts => ...)
  .WithNotParsed(errs => ...)
```

Coherently with `ParseArguments<T1, T2, ...>()` overloads used for verbs, you can take advantage also of `MapResult<T1, T2, ...>()`. Like in the sample with a single target instance, here we turn the parsed verb into an exit code:
```csharp
int Main(string[] args) {
  return Parser.Default.ParseArguments<AddOptions, CommitOptions, CloneOptions>(args)
    .MapResult(
      (AddOptions opts) => RunAddAndReturnExitCode(opts),
      (CommitOptions opts) => RunCommitAndReturnExitCode(opts),
      (CloneOptions opts) => RunCloneAndReturnExitCode(opts),
      errs => 1);
}
```

In this scenario the parser supplies you an additional `help` verb that allows:
```bash
$ app help clone
```
In this way application users can display specific verb command help screen.
```bash
$ app help
```
Or will display a help screen for available verbs.

## Immutable Options Type

If you develop according to functional programming, you probably won't define a mutable type like the ones presented in samples.

You're free to define an immutable type:
```csharp
class Options {
  private readonly IEnumerable<string> files;
  private readonly bool verbose;
  private readonly long offset;

  public Options(IEnumerable<string> files, bool verbose, long offset) {
    this.files = files;
    this.verbose = verbose;
    this.offset = offset;
  }

  [Option]
  public IEnumerable<string> Files { get { return files; } }

  [Option]
  public bool Verbose { get { return verbose; } }

  [Option]
  public long Offset { get { return offset; } ]
}
```

The parser will detect this class as immutable by the absence of public property setters and fields.

This is the same feature that allow you to parse against an **F#** record:
```fsharp
type options = {
  [<Option>] files : seq<string>;
  [<Option>] verbose : bool;
  [<Option>] offset : int64 option;
}
```

As you can see the `options.offset` record member was defined as `option<int64>` since the library has full support for `option<'a>` (full CLR name type name `Microsoft.FSharp.Core.FSharpOption<T>`).

## Help Screen

One of strengths of this library lies in the ability to automatically generate a help screen for the end user. See the [[Generating Help and Usage information]] page for more information. 

## Unparsing

You can transform back a parsed instance or a freshly created one into a string with command line arguments.
Assuming this options class:
```csharp
class Options {
  [Option('i',"input")] public string InputFile { get; set; }
  [Option('w')] public IEnumerable<string> Words { get; set; }
}
```
And building up this instance:
```csharp
var options = new Options { InputFile = "infile.csv", Words = new[] { "these", "are", "words" } };
```
You can format a command line string invoking:
```csharp
var arguments = CommandLine.Parser.Default.FormatCommandLine(options);
```
Output will be as above:
```
--input infile.csv -w these are words
```
In this first version of such feature the output is not customizable, but follows the above algorithm:
- options before values and sorted by name
- values sorted by index
- long name preferred over short name
- basic syntax: `name[space]value`
- strings with spaces and double quotes are correctly formatted and escaped

The feature will work with immutable instances and already supports **F#** `'T option` type. If the instance contains the `Verb` attribute, its name will be prepended before options.

If you need more control over output, you can use the following overload:
```csharp
class UnParserSettings {
  // Short or long name?
  bool PreferShortName { get; set; }
  // Group defined bool switches?
  bool GroupSwitches { get; set; }
  // Use equal sign with long name when possible?
  bool UseEqualToken { get; set; }
}

string FormatCommandLine<T>(T options, Action<UnParserSettings> configuration)
```
Example:
```csharp
var arguments = CommandLine.Parser.Default.FormatCommandLine(options, config => config.GroupSwitches = true);
```

## [Usage] Attribute

The `Usage` attribute is a new **2.0.x** feature that allows you to add a properly formatted `USAGE:` section to your help screen. One or more usage examples can be defined, by providing a static `IEnumerable<Example>` property annotated with the `[Usage]` attribute. 

```csharp
using CommandLine.Text;

class Options
{
    [Option("filename", Required = false, HelpText = "Input filename.")]
    public string filename { get; set; }

    [Usage(ApplicationAlias = "yourapp")]
    public static IEnumerable<Example> Examples
    {
        get
        {
            return new List<Example>() {
                new Example("Convert file to a trendy format", new Options { filename = "file.bin" })
            };
        }
    }
}
```
Will produce the following help text:
```bash
CommandLine 2.0.201-alpha
Copyright (c) 2005 - 2015 Giacomo Stelluti Scala
USAGE:
Convert file to a trendy format:
yourapp --filename file.bin

  --filename    Input filename.

  --help        Display this help screen.

  --version     Display version information.
  ```


More than one usage can be defined. It is also possible to format the displayed usage by providing a list of `UnParserSettings`. 

```csharp
class Options {
  // Normal options here.

  [Usage(ApplicationAlias = "yourapp")]
  public static IEnumerable<Example> Examples {
    get {
      yield return new Example("Normal scenario", new Options { InputFile = "file.bin", OutputFile = "out.bin" });
      yield return new Example("Logging warnings", UnParserSettings.WithGroupSwitchesOnly() , new Options { InputFile = "file.bin", LogWarning = true });
      yield return new Example("Logging errors", new[] { UnParserSettings.WithGroupSwitchesOnly(), UnParserSettings.WithUseEqualTokenOnly() }, new Options { InputFile = "file.bin", LogError = true });
    }
  }
}
```

When working with formatting styles, the important thing to know is that `UnParserSettings` is exactly the same type accepted by `Parser.FormatCommandLine<T>(T options, Action<UnParserSettings>)`; since this API is the same used internally to generate part of the example command line.

`UnParserSettings.WithGroupSwitchesOnly()` and `UnParserSettings.WithUseEqualTokenOnly()` are just factory methods to simplify the creation of an instance with the property in the name set to true.

If you're an experienced command line user, you're wondering how `AutoBuild()` will handle this data when you define `AssemblyUsage` attribute. It will follows the rules above:

1. Prints header (`SentenceBuilder.UsageHadingText`) if you've used `Usage` or `AssemblyUsage` attribute and such header isn't an empty string (default `USAGE:`).

2. Prints content provided by `AssemblyUsage` if defined.

3. Prints content provided by `Usage` if defined.

The above output is taken from a unit test.
```bash
CommandLine 2.0.201-alpha
Copyright (c) 2005 - 2015 Giacomo Stelluti Scala

ERROR(S):
  Option 'badoption' is unknown.

USAGE:
Cloning quietly:
  git clone --quiet https://github.com/gsscoder/railwaysharp
Cloning without hard links:
  git clone --no-hardlinks https://github.com/gsscoder/csharpx


  --no-hardlinks    Optimize the cloning process from a repository on a local 
                    filesystem by copying files.

  -q, --quiet       Suppress summary message.

  --help            Display this help screen.

  --version         Display version information.

  URLS (pos. 0)     A list of url(s) to clone.
```

If you build `HelpText` instance by your own, you can rely on three methods to gather `Usage` attribute data:
```csharp
static string RenderUsageText<T>(ParserResult<T> parserResult)
static string RenderUsageText<T>(ParserResult<T> parserResult, Func<Example, Example> mapperFunc)
static IEnumerable<string> RenderUsageTextAsLines<T>(ParserResult<T> parserResult, Func<Example, Example> mapperFunc)
```