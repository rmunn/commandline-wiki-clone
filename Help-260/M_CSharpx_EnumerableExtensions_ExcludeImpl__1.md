# EnumerableExtensions.ExcludeImpl(*T*) Method 
 

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static IEnumerable<T> ExcludeImpl<T>(
	IEnumerable<T> sequence,
	int startIndex,
	int count
)

```

**VB**<br />
``` VB
Private Shared Function ExcludeImpl(Of T) ( 
	sequence As IEnumerable(Of T),
	startIndex As Integer,
	count As Integer
) As IEnumerable(Of T)
```

**C++**<br />
``` C++
private:
generic<typename T>
static IEnumerable<T>^ ExcludeImpl(
	IEnumerable<T>^ sequence, 
	int startIndex, 
	int count
)
```

**F#**<br />
``` F#
private static member ExcludeImpl : 
        sequence : IEnumerable<'T> * 
        startIndex : int * 
        count : int -> IEnumerable<'T> 

```


#### Parameters
&nbsp;<dl><dt>sequence</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(*T*)<br /></dd><dt>startIndex</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">System.Int32</a><br /></dd><dt>count</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">System.Int32</a><br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*T*)

## See Also


#### Reference
<a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />