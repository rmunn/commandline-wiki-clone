# EnumerableExtensions.ExpectingCountYieldingImpl(*TSource*) Method 
 

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static IEnumerable<TSource> ExpectingCountYieldingImpl<TSource>(
	IEnumerable<TSource> source,
	int count,
	Func<int, int, Exception> errorSelector
)

```

**VB**<br />
``` VB
Private Shared Function ExpectingCountYieldingImpl(Of TSource) ( 
	source As IEnumerable(Of TSource),
	count As Integer,
	errorSelector As Func(Of Integer, Integer, Exception)
) As IEnumerable(Of TSource)
```

**C++**<br />
``` C++
private:
generic<typename TSource>
static IEnumerable<TSource>^ ExpectingCountYieldingImpl(
	IEnumerable<TSource>^ source, 
	int count, 
	Func<int, int, Exception^>^ errorSelector
)
```

**F#**<br />
``` F#
private static member ExpectingCountYieldingImpl : 
        source : IEnumerable<'TSource> * 
        count : int * 
        errorSelector : Func<int, int, Exception> -> IEnumerable<'TSource> 

```


#### Parameters
&nbsp;<dl><dt>source</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(*TSource*)<br /></dd><dt>count</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">System.Int32</a><br /></dd><dt>errorSelector</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-3" target="_blank">System.Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">Int32</a>, <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">Int32</a>, <a href="https://docs.microsoft.com/dotnet/api/system.exception" target="_blank">Exception</a>)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TSource</dt><dd /></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*TSource*)

## See Also


#### Reference
<a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />