WIP.  Need to show how to modify the parsing calls from old v1.9 to new v2.x

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