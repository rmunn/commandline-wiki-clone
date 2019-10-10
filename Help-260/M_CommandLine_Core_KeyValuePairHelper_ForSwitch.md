# KeyValuePairHelper.ForSwitch Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static IEnumerable<KeyValuePair<string, IEnumerable<string>>> ForSwitch(
	IEnumerable<Token> tokens
)
```

**VB**<br />
``` VB
Public Shared Function ForSwitch ( 
	tokens As IEnumerable(Of Token)
) As IEnumerable(Of KeyValuePair(Of String, IEnumerable(Of String)))
```

**C++**<br />
``` C++
public:
static IEnumerable<KeyValuePair<String^, IEnumerable<String^>^>>^ ForSwitch(
	IEnumerable<Token^>^ tokens
)
```

**F#**<br />
``` F#
static member ForSwitch : 
        tokens : IEnumerable<Token> -> IEnumerable<KeyValuePair<string, IEnumerable<string>>> 

```


#### Parameters
&nbsp;<dl><dt>tokens</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="T_CommandLine_Core_Token">Token</a>)<br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.keyvaluepair-2" target="_blank">KeyValuePair</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>, <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)))

## See Also


#### Reference
<a href="T_CommandLine_Core_KeyValuePairHelper">KeyValuePairHelper Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />