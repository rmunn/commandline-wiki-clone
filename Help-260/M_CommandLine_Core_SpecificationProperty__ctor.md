# SpecificationProperty Constructor 
 

Initializes a new instance of the <a href="T_CommandLine_Core_SpecificationProperty">SpecificationProperty</a> class

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private SpecificationProperty(
	Specification specification,
	PropertyInfo property,
	Maybe<Object> value
)
```

**VB**<br />
``` VB
Private Sub New ( 
	specification As Specification,
	property As PropertyInfo,
	value As Maybe(Of Object)
)
```

**C++**<br />
``` C++
private:
SpecificationProperty(
	Specification^ specification, 
	PropertyInfo^ property, 
	Maybe<Object^>^ value
)
```

**F#**<br />
``` F#
new : 
        specification : Specification * 
        property : PropertyInfo * 
        value : Maybe<Object> -> SpecificationProperty
```


#### Parameters
&nbsp;<dl><dt>specification</dt><dd>Type: <a href="T_CommandLine_Core_Specification">CommandLine.Core.Specification</a><br /></dd><dt>property</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.reflection.propertyinfo" target="_blank">System.Reflection.PropertyInfo</a><br /></dd><dt>value</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>)<br /></dd></dl>

## See Also


#### Reference
<a href="T_CommandLine_Core_SpecificationProperty">SpecificationProperty Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />