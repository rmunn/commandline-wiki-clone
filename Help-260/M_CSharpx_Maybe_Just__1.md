# Maybe.Just(*T*) Method 
 

Builds the case when <a href="T_CSharpx_Maybe">Maybe</a> contains a value.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Just<T> Just<T>(
	T value
)

```

**VB**<br />
``` VB
Public Shared Function Just(Of T) ( 
	value As T
) As Just(Of T)
```

**C++**<br />
``` C++
public:
generic<typename T>
static Just<T>^ Just(
	T value
)
```

**F#**<br />
``` F#
static member Just : 
        value : 'T -> Just<'T> 

```


#### Parameters
&nbsp;<dl><dt>value</dt><dd>Type: *T*<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: <a href="T_CSharpx_Just_1">Just</a>(*T*)

## See Also


#### Reference
<a href="T_CSharpx_Maybe">Maybe Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />