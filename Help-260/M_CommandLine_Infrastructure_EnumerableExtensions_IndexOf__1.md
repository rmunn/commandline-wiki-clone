# EnumerableExtensions.IndexOf(*TSource*) Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Infrastructure">CommandLine.Infrastructure</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static int IndexOf<TSource>(
	this IEnumerable<TSource> source,
	Func<TSource, bool> predicate
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function IndexOf(Of TSource) ( 
	source As IEnumerable(Of TSource),
	predicate As Func(Of TSource, Boolean)
) As Integer
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename TSource>
static int IndexOf(
	IEnumerable<TSource>^ source, 
	Func<TSource, bool>^ predicate
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member IndexOf : 
        source : IEnumerable<'TSource> * 
        predicate : Func<'TSource, bool> -> int 

```


#### Parameters
&nbsp;<dl><dt>source</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(*TSource*)<br /></dd><dt>predicate</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(*TSource*, <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">Boolean</a>)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>TSource</dt><dd /></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">Int32</a>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*TSource*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Infrastructure_EnumerableExtensions">EnumerableExtensions Class</a><br /><a href="N_CommandLine_Infrastructure">CommandLine.Infrastructure Namespace</a><br />