# TypeInfo.Create Method (Type, IEnumerable(Type))
 

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
internal static TypeInfo Create(
	Type current,
	IEnumerable<Type> choices
)
```

**VB**<br />
``` VB
Friend Shared Function Create ( 
	current As Type,
	choices As IEnumerable(Of Type)
) As TypeInfo
```

**C++**<br />
``` C++
internal:
static TypeInfo^ Create(
	Type^ current, 
	IEnumerable<Type^>^ choices
)
```

**F#**<br />
``` F#
internal static member Create : 
        current : Type * 
        choices : IEnumerable<Type> -> TypeInfo 

```


#### Parameters
&nbsp;<dl><dt>current</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">System.Type</a><br /></dd><dt>choices</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a>)<br /></dd></dl>

#### Return Value
Type: <a href="T_CommandLine_TypeInfo">TypeInfo</a>

## See Also


#### Reference
<a href="T_CommandLine_TypeInfo">TypeInfo Class</a><br /><a href="Overload_CommandLine_TypeInfo_Create">Create Overload</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />