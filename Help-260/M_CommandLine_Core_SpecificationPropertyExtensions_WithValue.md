# SpecificationPropertyExtensions.WithValue Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static SpecificationProperty WithValue(
	this SpecificationProperty specProp,
	Maybe<Object> newValue
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function WithValue ( 
	specProp As SpecificationProperty,
	newValue As Maybe(Of Object)
) As SpecificationProperty
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
static SpecificationProperty^ WithValue(
	SpecificationProperty^ specProp, 
	Maybe<Object^>^ newValue
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member WithValue : 
        specProp : SpecificationProperty * 
        newValue : Maybe<Object> -> SpecificationProperty 

```


#### Parameters
&nbsp;<dl><dt>specProp</dt><dd>Type: <a href="T_CommandLine_Core_SpecificationProperty">CommandLine.Core.SpecificationProperty</a><br /></dd><dt>newValue</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>)<br /></dd></dl>

#### Return Value
Type: <a href="T_CommandLine_Core_SpecificationProperty">SpecificationProperty</a>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CommandLine_Core_SpecificationProperty">SpecificationProperty</a>. When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Core_SpecificationPropertyExtensions">SpecificationPropertyExtensions Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />