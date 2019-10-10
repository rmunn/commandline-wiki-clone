# MaybeExtensions.GetValueOrDefault(*T*) Method 
 

If contains a values returns it, otherwise returns *noneValue*.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static T GetValueOrDefault<T>(
	this Maybe<T> maybe,
	T noneValue
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function GetValueOrDefault(Of T) ( 
	maybe As Maybe(Of T),
	noneValue As T
) As T
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T>
static T GetValueOrDefault(
	Maybe<T>^ maybe, 
	T noneValue
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member GetValueOrDefault : 
        maybe : Maybe<'T> * 
        noneValue : 'T -> 'T 

```


#### Parameters
&nbsp;<dl><dt>maybe</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(*T*)<br /></dd><dt>noneValue</dt><dd>Type: *T*<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: *T*

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CSharpx_Maybe_1">Maybe</a>(*T*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_MaybeExtensions">MaybeExtensions Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />