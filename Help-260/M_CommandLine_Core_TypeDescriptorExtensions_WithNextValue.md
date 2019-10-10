# TypeDescriptorExtensions.WithNextValue Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static TypeDescriptor WithNextValue(
	this TypeDescriptor descriptor,
	Maybe<TypeDescriptor> nextValue
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function WithNextValue ( 
	descriptor As TypeDescriptor,
	nextValue As Maybe(Of TypeDescriptor)
) As TypeDescriptor
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
static TypeDescriptor WithNextValue(
	TypeDescriptor descriptor, 
	Maybe<TypeDescriptor>^ nextValue
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member WithNextValue : 
        descriptor : TypeDescriptor * 
        nextValue : Maybe<TypeDescriptor> -> TypeDescriptor 

```


#### Parameters
&nbsp;<dl><dt>descriptor</dt><dd>Type: <a href="T_CommandLine_Core_TypeDescriptor">CommandLine.Core.TypeDescriptor</a><br /></dd><dt>nextValue</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(<a href="T_CommandLine_Core_TypeDescriptor">TypeDescriptor</a>)<br /></dd></dl>

#### Return Value
Type: <a href="T_CommandLine_Core_TypeDescriptor">TypeDescriptor</a>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CommandLine_Core_TypeDescriptor">TypeDescriptor</a>. When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Core_TypeDescriptorExtensions">TypeDescriptorExtensions Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />