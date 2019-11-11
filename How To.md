## Q1

**How to hide the options  --version /--help in the help text?**

**Answer:**

Use custom help and configure `HelText: AutoHelp=false and AutoVersion=false`

```csharp

void Main(string[] args)
{
  var parser = new Parser(with => with.HelpWriter = null);
  var parserResult = parser.ParseArguments<Options>(args);
  parserResult
    .WithParsed(opt => opt.Dump())
    .WithNotParsed(x =>
    {
      var helpText = HelpText.AutoBuild(parserResult, h =>
      {
        h.AutoHelp = false;     //hide --help
        h.AutoVersion = false;  //hide --version
        return HelpText.DefaultParsingErrorsHandler(parserResult, h);
      }, e => e);
      Console.WriteLine(helpText);
    });
}
```

**Note**:You need not to set Parser AutoHelp or AutoVersion.

----------

## Q2

**How to add dynamic contents which is calculated at runtime to help text?**

**Answer:**

Use custom help and configure `HelText:
`AddPostOptionsText (dynamic_dta)` : to be displayed before options

or
`AddPreOptionsText(dynamic_dta)` : to be displayed after options

```csharp
var helpText = HelpText.AutoBuild(parserResult, h =>
{
  h.AddPostOptionsText(dynamic_data);
  return HelpText.DefaultParsingErrorsHandler(parserResult, h);
}, e => e);
```

----------

## Q3

**What is the usage of EnableDashDash option in the Parser?**

**Answer:**

EnableDashDash option enable Parser to Stop processing arguments after '--' that start with dash '-' as named token and consider them  as a value token.

Example:

```cs
var parser = new Parser(with => {
  with.EnableDashDash = true;
});
```

Commandline example:

```
dosomething -- -a-file-that-starts-with-a-dash
```

Parser consider `-a-file-that-starts-with-a-dash`  as a value token.

----------

## Q4

**How to direct the default version screen or help screen to Console.Output?**

**Answer:**
The default version screen or help screen  is directed to Console.Error.
Use the custom Parser with the extension methods IsVersion() and IsHelp().

Code Example

```cs

 static void Main (string[] args) {
 	var helpWriter = new StringWriter ();
 	var parser = new CommandLine.Parser (with => with.HelpWriter = helpWriter);
 	parser.ParseArguments<Options> (args)
 		.WithParsed (opts => opts.Dump ())
 		.WithNotParsed (errs => DisplayHelp (errs, helpWriter));
 }

 static void DisplayHelp (IEnumerable<Error> errs, TextWriter helpWriter) {
 	if (errs.IsVersion () || errs.IsHelp ())
 		Console.WriteLine (helpWriter.ToString ());
 	else
 		Console.Error.WriteLine (helpWriter.ToString ());
 }

```

---------------

## Q5

**How to define Help Text for positional arguments?**

**Answer:**

Positional arguments are defined using ValueAttribute. Set  the `HelpText` property of the `ValueAttribute` with the help string.
Also, `MetaName` can be added to set the name of the positional value specification as described below:

```cs
[Value(0,MetaName = "InputPath",HelpText = "Input file-name including path")]
public string InputPath { get; set; }
```

Example:

```cs
public class Options {
  [Value(0,MetaName = "InputPath",HelpText = "Input file-name including path")]
  public string InputPath { get; set; }

  [Value(1,MetaName = "OutPath",HelpText = "Output file-name including path")]        
  public string OutputPath { get; set; }
}
```

The generated help screen is:

```
ConsoleApp 1.0.0
Copyright (C) 2019 ConsoleApp

  --help                Display this help screen.

  --version             Display version information.

  InputPath (pos. 0)    Input filename including path

  OutPath (pos. 1)      Output filename including path

```
This is applied also to the Named Options.

For more details of the `MetaName` and `MetaValue`, see [[API documentation|T_CommandLine_ValueAttribute#properties]]

---------

## Q6

**How to Print Help Screen when the Parser Success from within `WithParsed` Method?**

**Answer:**

- Declare `parserResult`

```cs
static ParserResult<Options> parserResult ;
```

- Pass `ParserResult` to the following method to generate the Help Text:

```cs
    // Use default configuration
		// You can customize HelpText and pass different configuratins
		//See wiki
		// https://github.com/commandlineparser/commandline/wiki/How-To#q1
		// https://github.com/commandlineparser/commandline/wiki/HelpText-Configuration
    
static string GetHelp<T>(ParserResult<T> parserResult )
	{
	   	return  HelpText.AutoBuild(parserResult, h =>h,e=>e);
	}
```

- Call `GetHelp` from  `WithParsed` method

<details>
<summary> Complete Code Example- Click to Expand</summary>
<p>

```c#

using System;
using System.Collections.Generic;
using CommandLine;
using CommandLine.Text;

//Print Help Screen when Parser success
public class Program
{
	static ParserResult<Options> parserResult;
	public static void Main()
	{
		string[] args = new[]{"--stdin", "123"};
		Console.WriteLine("Call help screen when Parser success");
		var parser = new CommandLine.Parser(with => with.HelpWriter = null);
		parserResult = Parser.Default.ParseArguments<Options>(args);
		parserResult.WithParsed(Run).WithNotParsed(errs => HandleErrors(errs));
	}

	static void HandleErrors(IEnumerable<Error> errs)
	{
		Console.WriteLine("Parser Fail");
	}

	private static void Run(Options options)
	{
		Console.WriteLine("parser SUCCESS");
		if (!validate(options))
		{
			Console.WriteLine("Validation fail");
			var helpText = GetHelp<Options>(parserResult);
			Console.WriteLine(helpText);
		}
	}

	//Generate Help text
	static string GetHelp<T>(ParserResult<T> result)
	{
		// use default configuration
		// you can customize HelpText and pass different configuratins
		//see wiki
		// https://github.com/commandlineparser/commandline/wiki/How-To#q1
		// https://github.com/commandlineparser/commandline/wiki/HelpText-Configuration
		return HelpText.AutoBuild(result, h => h, e => e);
	}

	//validate options
	static bool validate(Options options)
	{
		// do validation 
		if (options.FileName == null)
			return false;
		return true;
	}
}

class Options
{
	[Option(Default = false, HelpText = "Prints all messages to standard output.")]
	public bool Verbose
	{
		get;
		set;
	}

	[Option("stdin", Default = false, HelpText = "Read from stdin")]
	public bool stdin
	{
		get;
		set;
	}

	[Option("file", HelpText = "File name")]
	public string FileName
	{
		get;
		set;
	}

	[Value(0, MetaName = "offset", HelpText = "File offset.")]
	public long? Offset
	{
		get;
		set;
	}
}
```

</p>
</details>  

[<img src="media/tryit.png">](https://dotnetfiddle.net/ovpkf1)
