One of strengths of this library lies in the ability to automatically generate a help screen for the end user. This is formatted using common conventions of command line applications through the use of metadata defined in Option, Value and Verb attributes.

## Built-in support for `--help`

The library supplies a built-in `--help` switch that halts processing and displays the help screen. The help screen is also displayed when parsing process fails, along with clear and explicit description of every error encountered.

```
C:\> SimpleSample --help
[output here]
```

## Using verbs

**When using verbs, the library supplies a built-in help verb.** It displays the verbs index (with the list of all verbs) or, when invoked with another verb as argument, it will display the specific help screen of the requested verb.

```
C:\> GitSample help
[output here]
```

## Built in version reporting

The parser can also print version information (taken from assembly level attributes) using the built-in `--version` switch or the built-in `version` verb.

```
C:\> SimpleSample --version
[output here]
```

When using verbs, both `--version` and `version` verb will work.

```
C:\> GitSample version
[output here]
C:\> GitSample --version
[output here]
```

## Customizing help output

If you use the pre-built singleton, this is configured to print the help screen to `Console.Error`. You can change this setting, creating and configuring a Parser instance by your own:

```cs
var parser = new Parser(config => config.HelpWriter = Console.Out);
```

There's a great difference between 2.0 and previous stable(s), since the new version is the only that can handle and generate help for Value positional options. To avoid the standard naming of value pos. N (where N is ValueAttribute.Index), you can use the new `MetaName` property.

## Overriding the default behavior

If you want to manage the help screen by our own, just leave `ParserSettings.HelpWriter` not set and, when parsing fails, build and print your custom help screen. Also in such case, you're not forced to do everything from scratch: you can use the same types employed by the library that live in `CommandLine.Text` namespace.

```c#
var parser = new Parser(config => config.HelpWriter = null);
```

See also Usage attribute paragraph.