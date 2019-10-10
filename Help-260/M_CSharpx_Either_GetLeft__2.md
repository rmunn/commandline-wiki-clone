# Either.GetLeft(*TLeft*, *TRight*) Method 
 

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static TLeft GetLeft<TLeft, TRight>(
	this Either<TLeft, TRight> either
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Private Shared Function GetLeft(Of TLeft, TRight) ( 
	either As Either(Of TLeft, TRight)
) As TLeft
```

**C++**<br />
``` C++
private:
[ExtensionAttribute]
generic<typename TLeft, typename TRight>
static TLeft GetLeft(
	Either<TLeft, TRight>^ either
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
private static member GetLeft : 
        either : Either<'TLeft, 'TRight> -> 'TLeft 

```


#### Parameters
&nbsp;<dl><dt>either</dt><dd>Type: <a href="T_CSharpx_Either_2">CSharpx.Either</a>(*TLeft*, *TRight*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TLeft</dt><dd /><dt>TRight</dt><dd /></dl>

#### Return Value
Type: *TLeft*

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CSharpx_Either_2">Either</a>(*TLeft*, *TRight*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_Either">Either Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />