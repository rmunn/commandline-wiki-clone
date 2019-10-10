# EitherExtensions.Bimap(*TLeft*, *TRight*, *TLeft1*, *TRight1*) Method 
 

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Either<TLeft1, TRight1> Bimap<TLeft, TRight, TLeft1, TRight1>(
	this Either<TLeft, TRight> either,
	Func<TLeft, TLeft1> mapLeft,
	Func<TRight, TRight1> mapRight
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function Bimap(Of TLeft, TRight, TLeft1, TRight1) ( 
	either As Either(Of TLeft, TRight),
	mapLeft As Func(Of TLeft, TLeft1),
	mapRight As Func(Of TRight, TRight1)
) As Either(Of TLeft1, TRight1)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename TLeft, typename TRight, typename TLeft1, typename TRight1>
static Either<TLeft1, TRight1>^ Bimap(
	Either<TLeft, TRight>^ either, 
	Func<TLeft, TLeft1>^ mapLeft, 
	Func<TRight, TRight1>^ mapRight
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member Bimap : 
        either : Either<'TLeft, 'TRight> * 
        mapLeft : Func<'TLeft, 'TLeft1> * 
        mapRight : Func<'TRight, 'TRight1> -> Either<'TLeft1, 'TRight1> 

```


#### Parameters
&nbsp;<dl><dt>either</dt><dd>Type: <a href="T_CSharpx_Either_2">CSharpx.Either</a>(*TLeft*, *TRight*)<br /></dd><dt>mapLeft</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*TLeft*, *TLeft1*)<br /></dd><dt>mapRight</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*TRight*, *TRight1*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TLeft</dt><dd /><dt>TRight</dt><dd /><dt>TLeft1</dt><dd /><dt>TRight1</dt><dd /></dl>

#### Return Value
Type: <a href="T_CSharpx_Either_2">Either</a>(*TLeft1*, *TRight1*)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CSharpx_Either_2">Either</a>(*TLeft*, *TRight*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_EitherExtensions">EitherExtensions Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />