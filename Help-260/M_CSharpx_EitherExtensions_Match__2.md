# EitherExtensions.Match(*TLeft*, *TRight*) Method 
 

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static void Match<TLeft, TRight>(
	this Either<TLeft, TRight> either,
	Action<TLeft> ifLeft,
	Action<TRight> ifRight
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Sub Match(Of TLeft, TRight) ( 
	either As Either(Of TLeft, TRight),
	ifLeft As Action(Of TLeft),
	ifRight As Action(Of TRight)
)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename TLeft, typename TRight>
static void Match(
	Either<TLeft, TRight>^ either, 
	Action<TLeft>^ ifLeft, 
	Action<TRight>^ ifRight
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member Match : 
        either : Either<'TLeft, 'TRight> * 
        ifLeft : Action<'TLeft> * 
        ifRight : Action<'TRight> -> unit 

```


#### Parameters
&nbsp;<dl><dt>either</dt><dd>Type: <a href="T_CSharpx_Either_2">CSharpx.Either</a>(*TLeft*, *TRight*)<br /></dd><dt>ifLeft</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.action-1" target="_blank">System.Action</a>(*TLeft*)<br /></dd><dt>ifRight</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.action-1" target="_blank">System.Action</a>(*TRight*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TLeft</dt><dd /><dt>TRight</dt><dd /></dl>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CSharpx_Either_2">Either</a>(*TLeft*, *TRight*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_EitherExtensions">EitherExtensions Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />