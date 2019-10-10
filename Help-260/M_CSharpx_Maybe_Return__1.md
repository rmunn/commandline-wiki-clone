# Maybe.Return(*T*) Method 
 

Inject a value into the monadic <a href="T_CSharpx_Maybe_1">Maybe(T)</a> type.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Maybe<T> Return<T>(
	T value
)

```

**VB**<br />
``` VB
Public Shared Function Return(Of T) ( 
	value As T
) As Maybe(Of T)
```

**C++**<br />
``` C++
public:
generic<typename T>
static Maybe<T>^ Return(
	T value
)
```

**F#**<br />
``` F#
static member Return : 
        value : 'T -> Maybe<'T> 

```


#### Parameters
&nbsp;<dl><dt>value</dt><dd>Type: *T*<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: <a href="T_CSharpx_Maybe_1">Maybe</a>(*T*)

## See Also


#### Reference
<a href="T_CSharpx_Maybe">Maybe Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />