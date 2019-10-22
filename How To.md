## Q1 ##
**How to hide the options  --version /--help in the help text?**

**Answer:**
 
Use custom help and configure `HelText: AutoHelp=false and AutoVersion=false`

```csharp

	void Main(string[] args)
	{
		var parser = new CommandLine.Parser(with=>with.HelpWriter=null); 
		var parserResult = parser.ParseArguments<Options>(args);	
		parserResult.WithParsed<Options>(opt=>opt.Dump())
					.WithNotParsed(x=> 
					{		
	           var helpText=  HelpText.AutoBuild(parserResult, h =>
	           {
	               h.AutoHelp=false; //hide --help
	               h.AutoVersion=false;	 //hide --version	
	              return HelpText.DefaultParsingErrorsHandler(parserResult, h);
	           } , e=>e);	
					  Console.WriteLine(helpText);			  
				  });
	}

```

**Note**:You need not to set Parser AutoHelp or AutoVersion.

----------

## Q2 ##
**How to add dynamic contents which is calculated at runtime to help text?**

**Answer:**

Use custom help and configure `HelText: 
`AddPostOptionsText (dynamic_dta)` : to be displayed before options 

or 
`AddPreOptionsText(dynamic_dta)` : to be displayed after options 


```csharp
  var helpText=  HelpText.AutoBuild(parserResult, h =>
	           {
	               h.AddPostOptionsText(dynamic_data);	              	
	              return HelpText.DefaultParsingErrorsHandler(parserResult, h);
	           } , e=>e);
```

----------

## Q3 ##
**What is the usage of EnableDashDash option in the Parser?**

**Answer:**

EnableDashDash option enable Parser to Stop processing arguments after '--' that start with dash '-' as named token and consider them  as a value token.

Example:

     var parser = new Parser(with => {
		with.EnableDashDash = true;
	});

Commandline example:

         dosomething -- -a-file-that-starts-with-a-dash
         
Parser consider   `-a-file-that-starts-with-a-dash`  as a value token.
       	