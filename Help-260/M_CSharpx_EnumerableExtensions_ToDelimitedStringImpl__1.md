# EnumerableExtensions.ToDelimitedStringImpl(*T*) Method 
 

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static string ToDelimitedStringImpl<T>(
	IEnumerable<T> source,
	string delimiter,
	Func<StringBuilder, T, StringBuilder> append
)

```

**VB**<br />
``` VB
Private Shared Function ToDelimitedStringImpl(Of T) ( 
	source As IEnumerable(Of T),
	delimiter As String,
	append As Func(Of StringBuilder, T, StringBuilder)
) As String
```

**C++**<br />
``` C++
private:
generic<typename T>
static String^ ToDelimitedStringImpl(
	IEnumerable<T>^ source, 
	String^ delimiter, 
	Func<StringBuilder^, T, StringBuilder^>^ append
)
```

**F#**<br />
``` F#
private static member ToDelimitedStringImpl : 
        source : IEnumerable<'T> * 
        delimiter : string * 
        append : Func<StringBuilder, 'T, StringBuilder> -> string 

```


#### Parameters
&nbsp;<dl><dt>source</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(*T*)<br /></dd><dt>delimiter</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>append</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-3" target="_blank">System.Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.text.stringbuilder" target="_blank">StringBuilder</a>, *T*, <a href="https://docs.microsoft.com/dotnet/api/system.text.stringbuilder" target="_blank">StringBuilder</a>)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>

## See Also


#### Reference
<a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />