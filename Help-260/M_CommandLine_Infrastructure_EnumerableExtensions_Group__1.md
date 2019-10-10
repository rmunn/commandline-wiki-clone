# EnumerableExtensions.Group(*T*) Method 
 

Breaks a collection into groups of a specified size.

**Namespace:**&nbsp;<a href="N_CommandLine_Infrastructure">CommandLine.Infrastructure</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static IEnumerable<T[]> Group<T>(
	this IEnumerable<T> source,
	int groupSize
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function Group(Of T) ( 
	source As IEnumerable(Of T),
	groupSize As Integer
) As IEnumerable(Of T())
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T>
static IEnumerable<array<T>^>^ Group(
	IEnumerable<T>^ source, 
	int groupSize
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member Group : 
        source : IEnumerable<'T> * 
        groupSize : int -> IEnumerable<'T[]> 

```


#### Parameters
&nbsp;<dl><dt>source</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(*T*)<br />A collection of .</dd><dt>groupSize</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">System.Int32</a><br />The number of items each group shall contain.</dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*T*[])<br />An enumeration of T[].

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(*T*). When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## Remarks
An incomplete group at the end of the source collection will be silently dropped.

## See Also


#### Reference
<a href="T_CommandLine_Infrastructure_EnumerableExtensions">EnumerableExtensions Class</a><br /><a href="N_CommandLine_Infrastructure">CommandLine.Infrastructure Namespace</a><br />