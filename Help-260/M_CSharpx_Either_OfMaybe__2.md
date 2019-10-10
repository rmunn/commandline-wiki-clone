# Either.OfMaybe(*TLeft*, *TRight*) Method 
 

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Either<TLeft, TRight> OfMaybe<TLeft, TRight>(
	Maybe<TRight> maybe,
	TLeft left
)

```

**VB**<br />
``` VB
Public Shared Function OfMaybe(Of TLeft, TRight) ( 
	maybe As Maybe(Of TRight),
	left As TLeft
) As Either(Of TLeft, TRight)
```

**C++**<br />
``` C++
public:
generic<typename TLeft, typename TRight>
static Either<TLeft, TRight>^ OfMaybe(
	Maybe<TRight>^ maybe, 
	TLeft left
)
```

**F#**<br />
``` F#
static member OfMaybe : 
        maybe : Maybe<'TRight> * 
        left : 'TLeft -> Either<'TLeft, 'TRight> 

```


#### Parameters
&nbsp;<dl><dt>maybe</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(*TRight*)<br /></dd><dt>left</dt><dd>Type: *TLeft*<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TLeft</dt><dd /><dt>TRight</dt><dd /></dl>

#### Return Value
Type: <a href="T_CSharpx_Either_2">Either</a>(*TLeft*, *TRight*)

## See Also


#### Reference
<a href="T_CSharpx_Either">Either Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />