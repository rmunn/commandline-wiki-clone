# EitherExtensions.ToEither(*TRight*) Method 
 

Equivalent to monadic <a href="M_CSharpx_Either_Return__1">Return(TRight)(TRight)</a> operation. Builds a <a href="T_CSharpx_Right_2">Right(TLeft, TRight)</a> value in case *value* by default.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Either<string, TRight> ToEither<TRight>(
	this TRight value
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function ToEither(Of TRight) ( 
	value As TRight
) As Either(Of String, TRight)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename TRight>
static Either<String^, TRight>^ ToEither(
	TRight value
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member ToEither : 
        value : 'TRight -> Either<string, 'TRight> 

```


#### Parameters
&nbsp;<dl><dt>value</dt><dd>Type: *TRight*<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TRight</dt><dd /></dl>

#### Return Value
Type: <a href="T_CSharpx_Either_2">Either</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>, *TRight*)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type . When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_EitherExtensions">EitherExtensions Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />