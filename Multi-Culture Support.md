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

## Using Double.PositiveInfinity
Double infinity `∞` which is represented by the constant `Double.PositiveInfinity` is not supported in Parser.Default because it uses `CultureInfo.InvariantCulture`.

To parse the Infinity ∞ , you should use custom parser and set ParsingCulture, like 'en-Us':
```cs
var parser = new Parser(with =>
        {          
            //setup culture for parser 'en-US', for example
            with.ParsingCulture = new CultureInfo("en-US"); //modify to use your cultureinfo
        });
var result = parser.ParseArguments<Options>(args);
```
### Example
```
-e ∞ -m 50 -p -w 0.25
```
If you want to use `Parser.Default`, you can use `Infinity` as a symbol value, e.g.
```
#-e ∞ -m 50 -p -w 0.25  //∞ not supported in Parser.Default
-e Infinity -m 50 -p -w 0.25  # use Infinity instead of  ∞
```

[<img src="media/tryit.png">](https://dotnetfiddle.net/Q1YA6Y)


## Setting CultureInfo in Console application

```cs
CultureInfo ci = new CultureInfo("it-IT");
Thread.CurrentThread.CurrentCulture = ci;
Thread.CurrentThread.CurrentUICulture = ci;
```


# See also

- [[Help Localization]]
