# KeyValuePairHelper.ToKeyValuePair Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static KeyValuePair<string, IEnumerable<string>> ToKeyValuePair(
	this string value,
	params string[] values
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Private Shared Function ToKeyValuePair ( 
	value As String,
	ParamArray values As String()
) As KeyValuePair(Of String, IEnumerable(Of String))
```

**C++**<br />
``` C++
private:
[ExtensionAttribute]
static KeyValuePair<String^, IEnumerable<String^>^> ToKeyValuePair(
	String^ value, 
	... array<String^>^ values
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
private static member ToKeyValuePair : 
        value : string * 
        values : string[] -> KeyValuePair<string, IEnumerable<string>> 

```


#### Parameters
&nbsp;<dl><dt>value</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>values</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a>[]<br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.keyvaluepair-2" target="_blank">KeyValuePair</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>, <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>))

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>. When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Core_KeyValuePairHelper">KeyValuePairHelper Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />