# EnumerableExtensions.Concat(*T*) Method (IEnumerable(*T*), *T*)
 

Returns a sequence consisting of the head elements and the given tail element.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static IEnumerable<T> Concat<T>(
	this IEnumerable<T> head,
	T tail
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function Concat(Of T) ( 
	head As IEnumerable(Of T),
	tail As T
) As IEnumerable(Of T)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T>
static IEnumerable<T>^ Concat(
	IEnumerable<T>^ head, 
	T tail
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member Concat : 
        head : IEnumerable<'T> * 
        tail : 'T -> IEnumerable<'T> 

```


#### Parameters
&nbsp;<dl><dt>head</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(*T*)<br /></dd><dt>tail</dt><dd>Type: *T*<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*T*)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*T*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions Class</a><br /><a href="Overload_CSharpx_EnumerableExtensions_Concat">Concat Overload</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />