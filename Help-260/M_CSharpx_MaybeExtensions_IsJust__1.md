# MaybeExtensions.IsJust(*T*) Method 
 

Returns `true` iffits argument is of the form <a href="T_CSharpx_Just_1">Just(T)</a>.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static bool IsJust<T>(
	this Maybe<T> maybe
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function IsJust(Of T) ( 
	maybe As Maybe(Of T)
) As Boolean
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T>
static bool IsJust(
	Maybe<T>^ maybe
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member IsJust : 
        maybe : Maybe<'T> -> bool 

```


#### Parameters
&nbsp;<dl><dt>maybe</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(*T*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">Boolean</a>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CSharpx_Maybe_1">Maybe</a>(*T*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_MaybeExtensions">MaybeExtensions Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />