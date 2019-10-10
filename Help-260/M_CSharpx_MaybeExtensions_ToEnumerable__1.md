# MaybeExtensions.ToEnumerable(*T*) Method 
 

Returns an empty list when given <a href="T_CSharpx_Nothing_1">Nothing(T)</a> or a singleton list when given a <a href="T_CSharpx_Just_1">Just(T)</a>.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static IEnumerable<T> ToEnumerable<T>(
	this Maybe<T> maybe
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function ToEnumerable(Of T) ( 
	maybe As Maybe(Of T)
) As IEnumerable(Of T)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T>
static IEnumerable<T>^ ToEnumerable(
	Maybe<T>^ maybe
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member ToEnumerable : 
        maybe : Maybe<'T> -> IEnumerable<'T> 

```


#### Parameters
&nbsp;<dl><dt>maybe</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(*T*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*T*)

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CSharpx_Maybe_1">Maybe</a>(*T*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_MaybeExtensions">MaybeExtensions Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />