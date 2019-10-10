# Either.GetLeftOrDefault(*TLeft*, *TRight*) Method 
 

Returns a Either Left or a defualt value.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static TLeft GetLeftOrDefault<TLeft, TRight>(
	Either<TLeft, TRight> either,
	TLeft default
)

```

**VB**<br />
``` VB
Public Shared Function GetLeftOrDefault(Of TLeft, TRight) ( 
	either As Either(Of TLeft, TRight),
	default As TLeft
) As TLeft
```

**C++**<br />
``` C++
public:
generic<typename TLeft, typename TRight>
static TLeft GetLeftOrDefault(
	Either<TLeft, TRight>^ either, 
	TLeft default
)
```

**F#**<br />
``` F#
static member GetLeftOrDefault : 
        either : Either<'TLeft, 'TRight> * 
        default : 'TLeft -> 'TLeft 

```


#### Parameters
&nbsp;<dl><dt>either</dt><dd>Type: <a href="T_CSharpx_Either_2">CSharpx.Either</a>(*TLeft*, *TRight*)<br /></dd><dt>default</dt><dd>Type: *TLeft*<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TLeft</dt><dd /><dt>TRight</dt><dd /></dl>

#### Return Value
Type: *TLeft*

## See Also


#### Reference
<a href="T_CSharpx_Either">Either Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />