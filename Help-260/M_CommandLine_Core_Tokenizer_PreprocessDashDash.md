# Tokenizer.PreprocessDashDash Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Result<IEnumerable<Token>, Error> PreprocessDashDash(
	IEnumerable<string> arguments,
	Func<IEnumerable<string>, Result<IEnumerable<Token>, Error>> tokenizer
)
```

**VB**<br />
``` VB
Public Shared Function PreprocessDashDash ( 
	arguments As IEnumerable(Of String),
	tokenizer As Func(Of IEnumerable(Of String), Result(Of IEnumerable(Of Token), Error))
) As Result(Of IEnumerable(Of Token), Error)
```

**C++**<br />
``` C++
public:
static Result<IEnumerable<Token^>^, Error^>^ PreprocessDashDash(
	IEnumerable<String^>^ arguments, 
	Func<IEnumerable<String^>^, Result<IEnumerable<Token^>^, Error^>^>^ tokenizer
)
```

**F#**<br />
``` F#
static member PreprocessDashDash : 
        arguments : IEnumerable<string> * 
        tokenizer : Func<IEnumerable<string>, Result<IEnumerable<Token>, Error>> -> Result<IEnumerable<Token>, Error> 

```


#### Parameters
&nbsp;<dl><dt>arguments</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)<br /></dd><dt>tokenizer</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>), <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Core_Token">Token</a>), <a href="T_CommandLine_Error">Error</a>))<br /></dd></dl>

#### Return Value
Type: <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Core_Token">Token</a>), <a href="T_CommandLine_Error">Error</a>)

## See Also


#### Reference
<a href="T_CommandLine_Core_Tokenizer">Tokenizer Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />