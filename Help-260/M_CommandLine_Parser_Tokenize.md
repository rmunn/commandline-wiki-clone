# Parser.Tokenize Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static Result<IEnumerable<Token>, Error> Tokenize(
	IEnumerable<string> arguments,
	IEnumerable<OptionSpecification> optionSpecs,
	ParserSettings settings
)
```

**VB**<br />
``` VB
Private Shared Function Tokenize ( 
	arguments As IEnumerable(Of String),
	optionSpecs As IEnumerable(Of OptionSpecification),
	settings As ParserSettings
) As Result(Of IEnumerable(Of Token), Error)
```

**C++**<br />
``` C++
private:
static Result<IEnumerable<Token^>^, Error^>^ Tokenize(
	IEnumerable<String^>^ arguments, 
	IEnumerable<OptionSpecification^>^ optionSpecs, 
	ParserSettings^ settings
)
```

**F#**<br />
``` F#
private static member Tokenize : 
        arguments : IEnumerable<string> * 
        optionSpecs : IEnumerable<OptionSpecification> * 
        settings : ParserSettings -> Result<IEnumerable<Token>, Error> 

```


#### Parameters
&nbsp;<dl><dt>arguments</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)<br /></dd><dt>optionSpecs</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="T_CommandLine_Core_OptionSpecification">OptionSpecification</a>)<br /></dd><dt>settings</dt><dd>Type: <a href="T_CommandLine_ParserSettings">CommandLine.ParserSettings</a><br /></dd></dl>

#### Return Value
Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Core_Token">Token</a>), <a href="T_CommandLine_Error">Error</a>)

## See Also


#### Reference
<a href="T_CommandLine_Parser">Parser Class</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />