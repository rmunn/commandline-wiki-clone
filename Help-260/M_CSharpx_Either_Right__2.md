# Either.Right(*TLeft*, *TRight*) Method 
 

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Either<TLeft, TRight> Right<TLeft, TRight>(
	TRight value
)

```

**VB**<br />
``` VB
Public Shared Function Right(Of TLeft, TRight) ( 
	value As TRight
) As Either(Of TLeft, TRight)
```

**C++**<br />
``` C++
public:
generic<typename TLeft, typename TRight>
static Either<TLeft, TRight>^ Right(
	TRight value
)
```

**F#**<br />
``` F#
static member Right : 
        value : 'TRight -> Either<'TLeft, 'TRight> 

```


#### Parameters
&nbsp;<dl><dt>value</dt><dd>Type: *TRight*<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TLeft</dt><dd /><dt>TRight</dt><dd /></dl>

#### Return Value
Type: <a href="T_CSharpx_Either_2">Either</a>(*TLeft*, *TRight*)

## See Also


#### Reference
<a href="T_CSharpx_Either">Either Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />