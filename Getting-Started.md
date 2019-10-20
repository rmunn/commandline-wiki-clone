Firstly, install the package within the Package Manager in Visual Studio to download and setup references. (Tools, Nuget Package Manager, Package Manager Console)

```
PM> Install-Package CommandLineParser
```
You can use the next template for Console Project in VS 2017 or above:


      <Project Sdk="Microsoft.NET.Sdk">
         <PropertyGroup>
            <OutputType>Exe</OutputType>
            <TargetFramework>net461</TargetFramework>
            <!-- in case you are using Assemplyinfo.cs -->
	        <GenerateAssemblyInfo>false</GenerateAssemblyInfo>
         </PropertyGroup>
        <ItemGroup>  
           <PackageReference Include="CommandLineParser" Version="2.6.0" />
        </ItemGroup>
      </Project>

The Parser is activated from the `Parser` class, defined in the `CommandLine` namespace. I suggest that you use the pre-configured `Default` singleton, and only construct your own instance when really required.

```csharp
using CommandLine;

namespace GetStartedSample 
{
	static class Program
	{
       static void Main(string[] args)
       {
		// (1) default options
		var result = Parser.Default.ParseArguments<Options>(args);

		// or (2) build and configure instance
		var parser = new Parser(with => with.EnableDashDash = true);
		var result = parser.ParseArguments<Options>(args);
		
		Console.WriteLine("Hello World.");
      }
	}
}
```

In the latter case the `Parser(Action<ParserSettings>)` constructor was called to configure the parser via the `ParserSettings` instance.

For more information of ParserSettings, see [[API reference: ParserSettings|T_CommandLine_ParserSettings]]

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

[<img src="media/tryit.png">](https://dotnetfiddle.net/ZBSD2B)

For more information of ValueAttribe, see [[API reference: ValueAttribute|T_CommandLine_ValueAttribute]]

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

`Option` attribute also supports a `Separator` property to mimic the deprecated `OptionList` behaviour when applied to sequences.
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

[<img src="media/tryit.png">](https://dotnetfiddle.net/qMRBhH)

For more information of OptionAttribe, see [[API reference: OptionAttribute|T_CommandLine_OptionAttribute]]

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
static int Main(string[] args) {
  return Parser.Default.ParseArguments<Options>(args)
    .MapResult(
      options => RunAndReturnExitCode(options),
      _ => 1);
}
 static int	RunAndReturnExitCode(Options options)
	 {
		 options.Dump();
		 return 0;
	 }
```

`MapResult` provides a way to transform result data into another value and it can accept up to 16 parameter. Also `MapResult` can be used for async/await 

For more than 16 type, there is a ParseArgument() overload that takes an array of Types.

# Using MapResult in async/await

```csharp
 public class Program
    {
		public static async Task Main(string[] args)
		{			
                  
		   var result = Parser.Default.ParseArguments<Options>(args);			
	     var retCode=   await	result.MapResult(
         async options => await RunAndReturnExitCodeAsync(options),
         _ => Task.FromResult(1));
			Console.WriteLine($"retCode={retCode}");
		}  
		
		//async method
	 static async Task<int>	RunAndReturnExitCodeAsync(Options options)
	 {
		 options.Dump();
		 await Task.Delay(20);//simulate async method		
		 return 0;
	 }
    }
```

[<img src="media/tryit.png">](https://dotnetfiddle.net/IvOG57)