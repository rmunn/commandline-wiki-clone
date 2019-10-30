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