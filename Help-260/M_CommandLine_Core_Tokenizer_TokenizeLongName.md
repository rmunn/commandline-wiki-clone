# Tokenizer.TokenizeLongName Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static IEnumerable<Token> TokenizeLongName(
	string value,
	Action<Error> onError
)
```

**VB**<br />
``` VB
Private Shared Function TokenizeLongName ( 
	value As String,
	onError As Action(Of Error)
) As IEnumerable(Of Token)
```

**C++**<br />
``` C++
private:
static IEnumerable<Token^>^ TokenizeLongName(
	String^ value, 
	Action<Error^>^ onError
)
```

**F#**<br />
``` F#
private static member TokenizeLongName : 
        value : string * 
        onError : Action<Error> -> IEnumerable<Token> 

```


#### Parameters
&nbsp;<dl><dt>value</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>onError</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.action-1" target="_blank">System.Action</a>(<a href="T_CommandLine_Error">Error</a>)<br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Core_Token">Token</a>)

## See Also


#### Reference
<a href="T_CommandLine_Core_Tokenizer">Tokenizer Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />