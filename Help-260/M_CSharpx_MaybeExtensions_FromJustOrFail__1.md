# MaybeExtensions.FromJustOrFail(*T*) Method 
 

Extracts the element out of a <a href="T_CSharpx_Just_1">Just(T)</a> and throws an error if its argument is <a href="T_CSharpx_Nothing_1">Nothing(T)</a>.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static T FromJustOrFail<T>(
	this Maybe<T> maybe,
	Exception exceptionToThrow = null
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function FromJustOrFail(Of T) ( 
	maybe As Maybe(Of T),
	Optional exceptionToThrow As Exception = Nothing
) As T
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T>
static T FromJustOrFail(
	Maybe<T>^ maybe, 
	Exception^ exceptionToThrow = nullptr
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member FromJustOrFail : 
        maybe : Maybe<'T> * 
        ?exceptionToThrow : Exception 
(* Defaults:
        let _exceptionToThrow = defaultArg exceptionToThrow null
*)
-> 'T 

```


#### Parameters
&nbsp;<dl><dt>maybe</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(*T*)<br /></dd><dt>exceptionToThrow (Optional)</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.exception" target="_blank">System.Exception</a><br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: *T*

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CSharpx_Maybe_1">Maybe</a>(*T*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_MaybeExtensions">MaybeExtensions Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />