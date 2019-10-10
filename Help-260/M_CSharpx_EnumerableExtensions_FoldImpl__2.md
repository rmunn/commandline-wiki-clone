# EnumerableExtensions.FoldImpl(*T*, *TResult*) Method 
 

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static TResult FoldImpl<T, TResult>(
	IEnumerable<T> source,
	int count,
	Func<T, TResult> folder1,
	Func<T, T, TResult> folder2,
	Func<T, T, T, TResult> folder3,
	Func<T, T, T, T, TResult> folder4
)

```

**VB**<br />
``` VB
Private Shared Function FoldImpl(Of T, TResult) ( 
	source As IEnumerable(Of T),
	count As Integer,
	folder1 As Func(Of T, TResult),
	folder2 As Func(Of T, T, TResult),
	folder3 As Func(Of T, T, T, TResult),
	folder4 As Func(Of T, T, T, T, TResult)
) As TResult
```

**C++**<br />
``` C++
private:
generic<typename T, typename TResult>
static TResult FoldImpl(
	IEnumerable<T>^ source, 
	int count, 
	Func<T, TResult>^ folder1, 
	Func<T, T, TResult>^ folder2, 
	Func<T, T, T, TResult>^ folder3, 
	Func<T, T, T, T, TResult>^ folder4
)
```

**F#**<br />
``` F#
private static member FoldImpl : 
        source : IEnumerable<'T> * 
        count : int * 
        folder1 : Func<'T, 'TResult> * 
        folder2 : Func<'T, 'T, 'TResult> * 
        folder3 : Func<'T, 'T, 'T, 'TResult> * 
        folder4 : Func<'T, 'T, 'T, 'T, 'TResult> -> 'TResult 

```


#### Parameters
&nbsp;<dl><dt>source</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(*T*)<br /></dd><dt>count</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">System.Int32</a><br /></dd><dt>folder1</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*T*, *TResult*)<br /></dd><dt>folder2</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-3" target="_blank">System.Func</a>(*T*, *T*, *TResult*)<br /></dd><dt>folder3</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-4" target="_blank">System.Func</a>(*T*, *T*, *T*, *TResult*)<br /></dd><dt>folder4</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-5" target="_blank">System.Func</a>(*T*, *T*, *T*, *T*, *TResult*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /><dt>TResult</dt><dd /></dl>

#### Return Value
Type: *TResult*

## See Also


#### Reference
<a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />