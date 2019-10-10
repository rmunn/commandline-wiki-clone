# EnumerableExtensions.PairwiseImpl(*TSource*, *TResult*) Method 
 

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static IEnumerable<TResult> PairwiseImpl<TSource, TResult>(
	this IEnumerable<TSource> source,
	Func<TSource, TSource, TResult> resultSelector
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Private Shared Function PairwiseImpl(Of TSource, TResult) ( 
	source As IEnumerable(Of TSource),
	resultSelector As Func(Of TSource, TSource, TResult)
) As IEnumerable(Of TResult)
```

**C++**<br />
``` C++
private:
[ExtensionAttribute]
generic<typename TSource, typename TResult>
static IEnumerable<TResult>^ PairwiseImpl(
	IEnumerable<TSource>^ source, 
	Func<TSource, TSource, TResult>^ resultSelector
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
private static member PairwiseImpl : 
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