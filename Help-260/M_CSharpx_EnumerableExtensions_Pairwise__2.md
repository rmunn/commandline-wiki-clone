# EnumerableExtensions.Pairwise(*TSource*, *TResult*) Method 
 

Returns a sequence resulting from applying a function to each element in the source sequence and its predecessor, with the exception of the first element which is only returned as the predecessor of the second element.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static IEnumerable<TResult> Pairwise<TSource, TResult>(
	this IEnumerable<TSource> source,
	Func<TSource, TSource, TResult> resultSelector
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function Pairwise(Of TSource, TResult) ( 
	source As IEnumerable(Of TSource),
	resultSelector As Func(Of TSource, TSource, TResult)
) As IEnumerable(Of TResult)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename TSource, typename TResult>
static IEnumerable<TResult>^ Pairwise(
	IEnumerable<TSource>^ source, 
	Func<TSource, TSource, TResult>^ resultSelector
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member Pairwise : 
        source : IEnumerable<'TSource> * 
        resultSelector : Func<'TSource, 'TSource, 'TResult> -> IEnumerable<'TResult> 

```


#### Parameters
&nbsp;<dl><dt>source</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(*TSource*)<br /></dd><dt>resultSelector</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-3" target="_blank">System.Func</a>(*TSource*, *TSource*, *TResult*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TSource</dt><dd /><dt>TResult</dt><dd /></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*TResult*)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*TSource*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />