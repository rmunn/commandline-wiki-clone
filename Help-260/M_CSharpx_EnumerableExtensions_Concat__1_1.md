# EnumerableExtensions.Concat(*T*) Method (*T*, IEnumerable(*T*))
 

Returns a sequence consisting of the head element and the given tail elements.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static IEnumerable<T> Concat<T>(
	this T head,
	IEnumerable<T> tail
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function Concat(Of T) ( 
	head As T,
	tail As IEnumerable(Of T)
) As IEnumerable(Of T)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T>
static IEnumerable<T>^ Concat(
	T head, 
	IEnumerable<T>^ tail
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member Concat : 
        head : 'T * 
        tail : IEnumerable<'T> -> IEnumerable<'T> 

```


#### Parameters
&nbsp;<dl><dt>head</dt><dd>Type: *T*<br /></dd><dt>tail</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(*T*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*T*)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type . When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions Class</a><br /><a href="Overload_CSharpx_EnumerableExtensions_Concat">Concat Overload</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />