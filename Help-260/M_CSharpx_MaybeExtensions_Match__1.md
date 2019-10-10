# MaybeExtensions.Match(*T*) Method (Maybe(*T*), Action(*T*), Action)
 

Provides pattern matching using <a href="https://docs.microsoft.com/dotnet/api/system.action" target="_blank">Action</a> delegates.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static void Match<T>(
	this Maybe<T> maybe,
	Action<T> ifJust,
	Action ifNothing
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Sub Match(Of T) ( 
	maybe As Maybe(Of T),
	ifJust As Action(Of T),
	ifNothing As Action
)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T>
static void Match(
	Maybe<T>^ maybe, 
	Action<T>^ ifJust, 
	Action^ ifNothing
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member Match : 
        maybe : Maybe<'T> * 
        ifJust : Action<'T> * 
        ifNothing : Action -> unit 

```


#### Parameters
&nbsp;<dl><dt>maybe</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(*T*)<br /></dd><dt>ifJust</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.action-1" target="_blank">System.Action</a>(*T*)<br /></dd><dt>ifNothing</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.action" target="_blank">System.Action</a><br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CSharpx_Maybe_1">Maybe</a>(*T*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_MaybeExtensions">MaybeExtensions Class</a><br /><a href="Overload_CSharpx_MaybeExtensions_Match">Match Overload</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />