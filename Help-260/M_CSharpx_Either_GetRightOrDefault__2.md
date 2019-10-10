# Either.GetRightOrDefault(*TLeft*, *TRight*) Method 
 

Returns a Either Right or a defualt value.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static TRight GetRightOrDefault<TLeft, TRight>(
	Either<TLeft, TRight> either,
	TRight default
)

```

**VB**<br />
``` VB
Public Shared Function GetRightOrDefault(Of TLeft, TRight) ( 
	either As Either(Of TLeft, TRight),
	default As TRight
) As TRight
```

**C++**<br />
``` C++
public:
generic<typename TLeft, typename TRight>
static TRight GetRightOrDefault(
	Either<TLeft, TRight>^ either, 
	TRight default
)
```

**F#**<br />
``` F#
static member GetRightOrDefault : 
        either : Either<'TLeft, 'TRight> * 
        default : 'TRight -> 'TRight 

```


#### Parameters
&nbsp;<dl><dt>either</dt><dd>Type: <a href="T_CSharpx_Either_2">CSharpx.Either</a>(*TLeft*, *TRight*)<br /></dd><dt>default</dt><dd>Type: *TRight*<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TLeft</dt><dd /><dt>TRight</dt><dd /></dl>

#### Return Value
Type: *TRight*

## See Also


#### Reference
<a href="T_CSharpx_Either">Either Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />