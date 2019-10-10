# MaybeExtensions.Do(*T*) Method (Maybe(*T*), Action(*T*))
 

If contans a value executes an <a href="https://docs.microsoft.com/dotnet/api/system.action-1" target="_blank">Action(T)</a> delegate over it.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static void Do<T>(
	this Maybe<T> maybe,
	Action<T> action
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Sub Do(Of T) ( 
	maybe As Maybe(Of T),
	action As Action(Of T)
)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T>
static void Do(
	Maybe<T>^ maybe, 
	Action<T>^ action
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member Do : 
        maybe : Maybe<'T> * 
        action : Action<'T> -> unit 

```


#### Parameters
&nbsp;<dl><dt>maybe</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(*T*)<br /></dd><dt>action</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.action-1" target="_blank">System.Action</a>(*T*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CSharpx_Maybe_1">Maybe</a>(*T*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_MaybeExtensions">MaybeExtensions Class</a><br /><a href="Overload_CSharpx_MaybeExtensions_Do">Do Overload</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />