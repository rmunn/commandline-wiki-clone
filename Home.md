Version 2 is currently released as [![NuGet](https://img.shields.io/nuget/v/CommandLineParser.svg)](https://nuget.org/packages/CommandLineParser)



# Overview
- No dependencies! The standard `CommandLineParser` package has no dependencies.  If you want FSharp support, you should reference the `CommandLineParser.FSharp` package.
- [[Getting Started]] will show you how to get started with step-by-step instructions
- [[Generating Help and Usage information]] The library by default will automatically generate help and usage information for you.  
- [[Unparsing]] You can transform back a parsed instance or a freshly created one into a string with command line arguments.


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