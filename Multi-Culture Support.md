The parser is culture-aware. The args[] array passed to ParseArguments<T>(...) is a string array, so when the parser loads data into target instance every string undergoes a conversion.

Suppose you define an Option class like:
```cs
class Options {
  [Option('v', "value")]
  public double SomeValue { get; set; }
}
```
If your system use a dot as decimal separator and you type the following command line:
```
$ app -v 10,4
```

the parsing process will fail.

If you want that parsing occurs with a particular culture, just set desired CultureInfo in settings instance.
```cs

var parser = new CommandLine.Parser(with => with.ParsingCulture = new CultureInfo("it-IT"));
```

**Remarks:** CommandLine.Parser.Default is a singleton uses `CultureInfo.InvariantCulture`.

## Setting CultureInfo in Console application

```cs
CultureInfo ci = new CultureInfo("it-IT");
Thread.CurrentThread.CurrentCulture = ci;
Thread.CurrentThread.CurrentUICulture = ci;
```


# See also

- [[Help Localization]]
