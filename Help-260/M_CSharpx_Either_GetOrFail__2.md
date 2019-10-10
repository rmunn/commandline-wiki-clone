# Either.GetOrFail(*TLeft*, *TRight*) Method 
 

Returns a Either Right or fail with an exception.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static TRight GetOrFail<TLeft, TRight>(
	Either<TLeft, TRight> either
)

```

**VB**<br />
``` VB
Public Shared Function GetOrFail(Of TLeft, TRight) ( 
	either As Either(Of TLeft, TRight)
) As TRight
```

**C++**<br />
``` C++
public:
generic<typename TLeft, typename TRight>
static TRight GetOrFail(
	Either<TLeft, TRight>^ either
)
```

**F#**<br />
``` F#
static member GetOrFail : 
        either : Either<'TLeft, 'TRight> -> 'TRight 

```


#### Parameters
&nbsp;<dl><dt>either</dt><dd>Type: <a href="T_CSharpx_Either_2">CSharpx.Either</a>(*TLeft*, *TRight*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TLeft</dt><dd /><dt>TRight</dt><dd /></dl>

#### Return Value
Type: *TRight*

## See Also


#### Reference
<a href="T_CSharpx_Either">Either Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />