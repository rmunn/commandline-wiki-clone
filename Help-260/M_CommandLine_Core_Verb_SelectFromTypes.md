# Verb.SelectFromTypes Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static IEnumerable<Tuple<Verb, Type>> SelectFromTypes(
	IEnumerable<Type> types
)
```

**VB**<br />
``` VB
Public Shared Function SelectFromTypes ( 
	types As IEnumerable(Of Type)
) As IEnumerable(Of Tuple(Of Verb, Type))
```

**C++**<br />
``` C++
public:
static IEnumerable<Tuple<Verb^, Type^>^>^ SelectFromTypes(
	IEnumerable<Type^>^ types
)
```

**F#**<br />
``` F#
static member SelectFromTypes : 
        types : IEnumerable<Type> -> IEnumerable<Tuple<Verb, Type>> 

```


#### Parameters
&nbsp;<dl><dt>types</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a>)<br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.tuple-2" target="_blank">Tuple</a>(<a href="T_CommandLine_Core_Verb">Verb</a>, <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a>))

## See Also


#### Reference
<a href="T_CommandLine_Core_Verb">Verb Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />