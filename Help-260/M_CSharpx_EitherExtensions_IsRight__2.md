# EitherExtensions.IsRight(*TLeft*, *TRight*) Method 
 

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static bool IsRight<TLeft, TRight>(
	this Either<TLeft, TRight> either
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function IsRight(Of TLeft, TRight) ( 
	either As Either(Of TLeft, TRight)
) As Boolean
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename TLeft, typename TRight>
static bool IsRight(
	Either<TLeft, TRight>^ either
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member IsRight : 
        either : Either<'TLeft, 'TRight> -> bool 

```


#### Parameters
&nbsp;<dl><dt>either</dt><dd>Type: <a href="T_CSharpx_Either_2">CSharpx.Either</a>(*TLeft*, *TRight*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TLeft</dt><dd /><dt>TRight</dt><dd /></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">Boolean</a>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CSharpx_Either_2">Either</a>(*TLeft*, *TRight*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_EitherExtensions">EitherExtensions Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />