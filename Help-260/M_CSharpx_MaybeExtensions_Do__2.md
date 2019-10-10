# MaybeExtensions.Do(*T1*, *T2*) Method (Maybe(Tuple(*T1*, *T2*)), Action(*T1*, *T2*))
 

If contans a value executes an <a href="https://docs.microsoft.com/dotnet/api/system.action-2" target="_blank">Action(T1, T2)</a> delegate over it.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static void Do<T1, T2>(
	this Maybe<Tuple<T1, T2>> maybe,
	Action<T1, T2> action
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Sub Do(Of T1, T2) ( 
	maybe As Maybe(Of Tuple(Of T1, T2)),
	action As Action(Of T1, T2)
)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T1, typename T2>
static void Do(
	Maybe<Tuple<T1, T2>^>^ maybe, 
	Action<T1, T2>^ action
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member Do : 
        maybe : Maybe<Tuple<'T1, 'T2>> * 
        action : Action<'T1, 'T2> -> unit 

```


#### Parameters
&nbsp;<dl><dt>maybe</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.tuple-2" target="_blank">Tuple</a>(*T1*, *T2*))<br /></dd><dt>action</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.action-2" target="_blank">System.Action</a>(*T1*, *T2*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T1</dt><dd /><dt>T2</dt><dd /></dl>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CSharpx_Maybe_1">Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.tuple-2" target="_blank">Tuple</a>(*T1*, *T2*)). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_MaybeExtensions">MaybeExtensions Class</a><br /><a href="Overload_CSharpx_MaybeExtensions_Do">Do Overload</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />