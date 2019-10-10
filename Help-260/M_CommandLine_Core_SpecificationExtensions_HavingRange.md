# SpecificationExtensions.HavingRange Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static bool HavingRange(
	this Specification specification,
	Func<int, int, bool> predicate
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function HavingRange ( 
	specification As Specification,
	predicate As Func(Of Integer, Integer, Boolean)
) As Boolean
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
static bool HavingRange(
	Specification^ specification, 
	Func<int, int, bool>^ predicate
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member HavingRange : 
        specification : Specification * 
        predicate : Func<int, int, bool> -> bool 

```


#### Parameters
&nbsp;<dl><dt>specification</dt><dd>Type: <a href="T_CommandLine_Core_Specification">CommandLine.Core.Specification</a><br /></dd><dt>predicate</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-3" target="_blank">System.Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">Int32</a>, <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">Int32</a>, <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">Boolean</a>)<br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">Boolean</a>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CommandLine_Core_Specification">Specification</a>. When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Core_SpecificationExtensions">SpecificationExtensions Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />