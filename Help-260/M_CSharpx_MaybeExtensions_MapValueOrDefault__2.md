# MaybeExtensions.MapValueOrDefault(*T1*, *T2*) Method 
 

If contains a values executes a mapping function over it, otherwise returns *noneValue*.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static T2 MapValueOrDefault<T1, T2>(
	this Maybe<T1> maybe,
	Func<T1, T2> func,
	T2 noneValue
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function MapValueOrDefault(Of T1, T2) ( 
	maybe As Maybe(Of T1),
	func As Func(Of T1, T2),
	noneValue As T2
) As T2
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T1, typename T2>
static T2 MapValueOrDefault(
	Maybe<T1>^ maybe, 
	Func<T1, T2>^ func, 
	T2 noneValue
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member MapValueOrDefault : 
        maybe : Maybe<'T1> * 
        func : Func<'T1, 'T2> * 
        noneValue : 'T2 -> 'T2 

```


#### Parameters
&nbsp;<dl><dt>maybe</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(*T1*)<br /></dd><dt>func</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*T1*, *T2*)<br /></dd><dt>noneValue</dt><dd>Type: *T2*<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T1</dt><dd /><dt>T2</dt><dd /></dl>

#### Return Value
Type: *T2*

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CSharpx_Maybe_1">Maybe</a>(*T1*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_MaybeExtensions">MaybeExtensions Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />