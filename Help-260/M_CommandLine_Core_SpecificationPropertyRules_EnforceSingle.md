# SpecificationPropertyRules.EnforceSingle Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static Func<IEnumerable<SpecificationProperty>, IEnumerable<Error>> EnforceSingle(
	IEnumerable<Token> tokens
)
```

**VB**<br />
``` VB
Private Shared Function EnforceSingle ( 
	tokens As IEnumerable(Of Token)
) As Func(Of IEnumerable(Of SpecificationProperty), IEnumerable(Of Error))
```

**C++**<br />
``` C++
private:
static Func<IEnumerable<SpecificationProperty^>^, IEnumerable<Error^>^>^ EnforceSingle(
	IEnumerable<Token^>^ tokens
)
```

**F#**<br />
``` F#
private static member EnforceSingle : 
        tokens : IEnumerable<Token> -> Func<IEnumerable<SpecificationProperty>, IEnumerable<Error>> 

```


#### Parameters
&nbsp;<dl><dt>tokens</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="T_CommandLine_Core_Token">Token</a>)<br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Core_SpecificationProperty">SpecificationProperty</a>), <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Error">Error</a>))

## See Also


#### Reference
<a href="T_CommandLine_Core_SpecificationPropertyRules">SpecificationPropertyRules Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />