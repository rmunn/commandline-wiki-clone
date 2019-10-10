# EnumerableExtensions.Fold(*T*, *TResult*) Method (IEnumerable(*T*), Func(*T*, *TResult*))
 

Returns the result of applying a function to a sequence of 1 element.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static TResult Fold<T, TResult>(
	this IEnumerable<T> source,
	Func<T, TResult> folder
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function Fold(Of T, TResult) ( 
	source As IEnumerable(Of T),
	folder As Func(Of T, TResult)
) As TResult
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T, typename TResult>
static TResult Fold(
	IEnumerable<T>^ source, 
	Func<T, TResult>^ folder
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member Fold : 
        source : IEnumerable<'T> * 
        folder : Func<'T, 'TResult> -> 'TResult 

```


#### Parameters
&nbsp;<dl><dt>source</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(*T*)<br /></dd><dt>folder</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*T*, *TResult*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /><dt>TResult</dt><dd /></dl>

#### Return Value
Type: *TResult*

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*T*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions Class</a><br /><a href="Overload_CSharpx_EnumerableExtensions_Fold">Fold Overload</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />