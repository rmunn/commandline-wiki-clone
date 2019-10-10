# MaybeExtensions.Bind(*T1*, *T2*) Method 
 

Invokes a function on this maybe value that itself yields a maybe.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Maybe<T2> Bind<T1, T2>(
	this Maybe<T1> maybe,
	Func<T1, Maybe<T2>> func
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function Bind(Of T1, T2) ( 
	maybe As Maybe(Of T1),
	func As Func(Of T1, Maybe(Of T2))
) As Maybe(Of T2)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T1, typename T2>
static Maybe<T2>^ Bind(
	Maybe<T1>^ maybe, 
	Func<T1, Maybe<T2>^>^ func
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member Bind : 
        maybe : Maybe<'T1> * 
        func : Func<'T1, Maybe<'T2>> -> Maybe<'T2> 

```


#### Parameters
&nbsp;<dl><dt>maybe</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(*T1*)<br /></dd><dt>func</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*T1*, <a href="T_CSharpx_Maybe_1">Maybe</a>(*T2*))<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T1</dt><dd /><dt>T2</dt><dd /></dl>

#### Return Value
Type: <a href="T_CSharpx_Maybe_1">Maybe</a>(*T2*)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CSharpx_Maybe_1">Maybe</a>(*T1*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_MaybeExtensions">MaybeExtensions Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />