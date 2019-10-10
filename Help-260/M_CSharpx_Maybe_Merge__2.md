# Maybe.Merge(*T1*, *T2*) Method 
 

If both maybes contain a value, it merges them into a maybe with a tupled value.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Maybe<Tuple<T1, T2>> Merge<T1, T2>(
	Maybe<T1> first,
	Maybe<T2> second
)

```

**VB**<br />
``` VB
Public Shared Function Merge(Of T1, T2) ( 
	first As Maybe(Of T1),
	second As Maybe(Of T2)
) As Maybe(Of Tuple(Of T1, T2))
```

**C++**<br />
``` C++
public:
generic<typename T1, typename T2>
static Maybe<Tuple<T1, T2>^>^ Merge(
	Maybe<T1>^ first, 
	Maybe<T2>^ second
)
```

**F#**<br />
``` F#
static member Merge : 
        first : Maybe<'T1> * 
        second : Maybe<'T2> -> Maybe<Tuple<'T1, 'T2>> 

```


#### Parameters
&nbsp;<dl><dt>first</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(*T1*)<br /></dd><dt>second</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(*T2*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T1</dt><dd /><dt>T2</dt><dd /></dl>

#### Return Value
Type: <a href="T_CSharpx_Maybe_1">Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.tuple-2" target="_blank">Tuple</a>(*T1*, *T2*))

## See Also


#### Reference
<a href="T_CSharpx_Maybe">Maybe Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />