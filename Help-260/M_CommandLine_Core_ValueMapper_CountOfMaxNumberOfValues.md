# ValueMapper.CountOfMaxNumberOfValues Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static Maybe<int> CountOfMaxNumberOfValues(
	this Specification specification
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Private Shared Function CountOfMaxNumberOfValues ( 
	specification As Specification
) As Maybe(Of Integer)
```

**C++**<br />
``` C++
private:
[ExtensionAttribute]
static Maybe<int>^ CountOfMaxNumberOfValues(
	Specification^ specification
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
private static member CountOfMaxNumberOfValues : 
        specification : Specification -> Maybe<int> 

```


#### Parameters
&nbsp;<dl><dt>specification</dt><dd>Type: <a href="T_CommandLine_Core_Specification">CommandLine.Core.Specification</a><br /></dd></dl>

#### Return Value
Type: <a href="T_CSharpx_Maybe_1">Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">Int32</a>)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CommandLine_Core_Specification">Specification</a>. When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Core_ValueMapper">ValueMapper Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />