# Tokenizer.TokenizeShortName Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static IEnumerable<Token> TokenizeShortName(
	string value,
	Func<string, NameLookupResult> nameLookup
)
```

**VB**<br />
``` VB
Private Shared Function TokenizeShortName ( 
	value As String,
	nameLookup As Func(Of String, NameLookupResult)
) As IEnumerable(Of Token)
```

**C++**<br />
``` C++
private:
static IEnumerable<Token^>^ TokenizeShortName(
	String^ value, 
	Func<String^, NameLookupResult>^ nameLookup
)
```

**F#**<br />
``` F#
private static member TokenizeShortName : 
        value : string * 
        nameLookup : Func<string, NameLookupResult> -> IEnumerable<Token> 

```


#### Parameters
&nbsp;<dl><dt>value</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>nameLookup</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>, <a href="T_CommandLine_Core_NameLookupResult">NameLookupResult</a>)<br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Core_Token">Token</a>)

## See Also


#### Reference
<a href="T_CommandLine_Core_Tokenizer">Tokenizer Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />