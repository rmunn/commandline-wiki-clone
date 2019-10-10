# Switch.Partition Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static IEnumerable<Token> Partition(
	IEnumerable<Token> tokens,
	Func<string, Maybe<TypeDescriptor>> typeLookup
)
```

**VB**<br />
``` VB
Public Shared Function Partition ( 
	tokens As IEnumerable(Of Token),
	typeLookup As Func(Of String, Maybe(Of TypeDescriptor))
) As IEnumerable(Of Token)
```

**C++**<br />
``` C++
public:
static IEnumerable<Token^>^ Partition(
	IEnumerable<Token^>^ tokens, 
	Func<String^, Maybe<TypeDescriptor>^>^ typeLookup
)
```

**F#**<br />
``` F#
static member Partition : 
        tokens : IEnumerable<Token> * 
        typeLookup : Func<string, Maybe<TypeDescriptor>> -> IEnumerable<Token> 

```


#### Parameters
&nbsp;<dl><dt>tokens</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="T_CommandLine_Core_Token">Token</a>)<br /></dd><dt>typeLookup</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>, <a href="T_CSharpx_Maybe_1">Maybe</a>(<a href="T_CommandLine_Core_TypeDescriptor">TypeDescriptor</a>))<br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Core_Token">Token</a>)

## See Also


#### Reference
<a href="T_CommandLine_Core_Switch">Switch Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />