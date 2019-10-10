# EnumerableExtensions.ToDelimitedString(*TSource*) Method (IEnumerable(*TSource*))
 

Creates a delimited string from a sequence of values. The delimiter used depends on the current culture of the executing thread.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static string ToDelimitedString<TSource>(
	this IEnumerable<TSource> source
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function ToDelimitedString(Of TSource) ( 
	source As IEnumerable(Of TSource)
) As String
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename TSource>
static String^ ToDelimitedString(
	IEnumerable<TSource>^ source
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member ToDelimitedString : 
        source : IEnumerable<'TSource> -> string 

```


#### Parameters
&nbsp;<dl><dt>source</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(*TSource*)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TSource</dt><dd /></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*TSource*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions Class</a><br /><a href="Overload_CSharpx_EnumerableExtensions_ToDelimitedString">ToDelimitedString Overload</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />