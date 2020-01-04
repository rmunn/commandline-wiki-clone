# What is it?

**Unparsing** is being able to transform back a parsed instance or a freshly created one into a string with command line arguments.

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

## Skipping options with default values
When you have many command line parameters with default values in most of them you can  shorten the generated arguments.
This can be done by setting the configuration option `SkipDefault` to true in UnParserSettings (it's false by default):
```cs
SkipDefault =true;  //it's false by default
```
__Example__:
```cs
class Options
        {
            [Option(Default = 99)] //should be skipped when P1=99
            public  int P1 { get;set;}
            [Option()]
            public  string P2 { get;set;}
            [Option(Default = 88)] //should be skipped when P3=88
            public  int P3 { get;set;}
        }

var options = new Options{P2="xyz" ,P1=99, P3=88}	;

string args=  CommandLine.Parser.Default.FormatCommandLine(options, config=>config.SkipDefault =true);

//  args should be:  --p2 xyz   
```

__Note__:

- DatTime, TimeSpan and DateTimeOffset are formated as quoted string:
```
--start "1/4/2019 11:48:34 PM"
```
- When you use int Nullable type as option, the default value is null not 0.
In this case when we pass 0 to parameter it will be added to the arguments.

## UnParsing Demo

[<img src="media/tryit.png">](https://dotnetfiddle.net/8gPgBK)