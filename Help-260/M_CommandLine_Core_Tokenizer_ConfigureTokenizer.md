# Tokenizer.ConfigureTokenizer Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Func<IEnumerable<string>, IEnumerable<OptionSpecification>, Result<IEnumerable<Token>, Error>> ConfigureTokenizer(
	StringComparer nameComparer,
	bool ignoreUnknownArguments,
	bool enableDashDash
)
```

**VB**<br />
``` VB
Public Shared Function ConfigureTokenizer ( 
	nameComparer As StringComparer,
	ignoreUnknownArguments As Boolean,
	enableDashDash As Boolean
) As Func(Of IEnumerable(Of String), IEnumerable(Of OptionSpecification), Result(Of IEnumerable(Of Token), Error))
```

**C++**<br />
``` C++
public:
static Func<IEnumerable<String^>^, IEnumerable<OptionSpecification^>^, Result<IEnumerable<Token^>^, Error^>^>^ ConfigureTokenizer(
	StringComparer^ nameComparer, 
	bool ignoreUnknownArguments, 
	bool enableDashDash
)
```

**F#**<br />
``` F#
static member ConfigureTokenizer : 
        nameComparer : StringComparer * 
        ignoreUnknownArguments : bool * 
        enableDashDash : bool -> Func<IEnumerable<string>, IEnumerable<OptionSpecification>, Result<IEnumerable<Token>, Error>> 

```


#### Parameters
&nbsp;<dl><dt>nameComparer</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.stringcomparer" target="_blank">System.StringComparer</a><br /></dd><dt>ignoreUnknownArguments</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br /></dd><dt>enableDashDash</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-3" target="_blank">Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>), <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Core_OptionSpecification">OptionSpecification</a>), <a href="T_RailwaySharp_ErrorHandling_Result_2">Result</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Core_Token">Token</a>), <a href="T_CommandLine_Error">Error</a>))

## See Also


#### Reference
<a href="T_CommandLine_Core_Tokenizer">Tokenizer Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />