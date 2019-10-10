# EnumerableExtensions.ForEach(*T*) Method 
 

Immediately executes the given action on each element in the source sequence.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static void ForEach<T>(
	this IEnumerable<T> source,
	Action<T> action
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Sub ForEach(Of T) ( 
	source As IEnumerable(Of T),
	action As Action(Of T)
)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T>
static void ForEach(
	IEnumerable<T>^ source, 
	Action<T>^ action
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member ForEach : 
        source : IEnumerable<'T> * 
        action : Action<'T> -> unit 

```


#### Parameters
&nbsp;<dl><dt>source</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(*T*)<br /></dd><dt>action</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.action-1" target="_blank">System.Action</a>(*T*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd>The type of the elements in the sequence</dd></dl>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*T*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />