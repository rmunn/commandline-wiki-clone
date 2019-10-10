# NameExtensions.FromSpecification Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static NameInfo FromSpecification(
	this Specification specification
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function FromSpecification ( 
	specification As Specification
) As NameInfo
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
static NameInfo^ FromSpecification(
	Specification^ specification
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member FromSpecification : 
        specification : Specification -> NameInfo 

```


#### Parameters
&nbsp;<dl><dt>specification</dt><dd>Type: <a href="T_CommandLine_Core_Specification">CommandLine.Core.Specification</a><br /></dd></dl>

#### Return Value
Type: <a href="T_CommandLine_NameInfo">NameInfo</a>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CommandLine_Core_Specification">Specification</a>. When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Core_NameExtensions">NameExtensions Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />