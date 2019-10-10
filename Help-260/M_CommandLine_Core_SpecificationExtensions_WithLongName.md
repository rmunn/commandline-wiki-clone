# SpecificationExtensions.WithLongName Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static OptionSpecification WithLongName(
	this OptionSpecification specification,
	string newLongName
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function WithLongName ( 
	specification As OptionSpecification,
	newLongName As String
) As OptionSpecification
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
static OptionSpecification^ WithLongName(
	OptionSpecification^ specification, 
	String^ newLongName
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member WithLongName : 
        specification : OptionSpecification * 
        newLongName : string -> OptionSpecification 

```


#### Parameters
&nbsp;<dl><dt>specification</dt><dd>Type: <a href="T_CommandLine_Core_OptionSpecification">CommandLine.Core.OptionSpecification</a><br /></dd><dt>newLongName</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd></dl>

#### Return Value
Type: <a href="T_CommandLine_Core_OptionSpecification">OptionSpecification</a>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CommandLine_Core_OptionSpecification">OptionSpecification</a>. When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Core_SpecificationExtensions">SpecificationExtensions Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />