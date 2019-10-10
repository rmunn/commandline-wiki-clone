# TypeInfo Constructor 
 

Initializes a new instance of the <a href="T_CommandLine_TypeInfo">TypeInfo</a> class

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private TypeInfo(
	Type current,
	IEnumerable<Type> choices
)
```

**VB**<br />
``` VB
Private Sub New ( 
	current As Type,
	choices As IEnumerable(Of Type)
)
```

**C++**<br />
``` C++
private:
TypeInfo(
	Type^ current, 
	IEnumerable<Type^>^ choices
)
```

**F#**<br />
``` F#
new : 
        current : Type * 
        choices : IEnumerable<Type> -> TypeInfo
```


#### Parameters
&nbsp;<dl><dt>current</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">System.Type</a><br /></dd><dt>choices</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a>)<br /></dd></dl>

## See Also


#### Reference
<a href="T_CommandLine_TypeInfo">TypeInfo Class</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />