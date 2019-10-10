# Tokenizer.Normalize Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static IEnumerable<Token> Normalize(
	IEnumerable<Token> tokens,
	Func<string, bool> nameLookup
)
```

**VB**<br />
``` VB
Public Shared Function Normalize ( 
	tokens As IEnumerable(Of Token),
	nameLookup As Func(Of String, Boolean)
) As IEnumerable(Of Token)
```

**C++**<br />
``` C++
public:
static IEnumerable<Token^>^ Normalize(
	IEnumerable<Token^>^ tokens, 
	Func<String^, bool>^ nameLookup
)
```

**F#**<br />
``` F#
static member Normalize : 
        tokens : IEnumerable<Token> * 
        nameLookup : Func<string, bool> -> IEnumerable<Token> 

```


#### Parameters
&nbsp;<dl><dt>tokens</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="T_CommandLine_Core_Token">Token</a>)<br /></dd><dt>nameLookup</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>, <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">Boolean</a>)<br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Core_Token">Token</a>)

## See Also


#### Reference
<a href="T_CommandLine_Core_Tokenizer">Tokenizer Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />