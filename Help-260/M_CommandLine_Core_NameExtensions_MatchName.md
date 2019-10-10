# NameExtensions.MatchName Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static bool MatchName(
	this string value,
	string shortName,
	string longName,
	StringComparer comparer
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function MatchName ( 
	value As String,
	shortName As String,
	longName As String,
	comparer As StringComparer
) As Boolean
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
static bool MatchName(
	String^ value, 
	String^ shortName, 
	String^ longName, 
	StringComparer^ comparer
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member MatchName : 
        value : string * 
        shortName : string * 
        longName : string * 
        comparer : StringComparer -> bool 

```


#### Parameters
&nbsp;<dl><dt>value</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>shortName</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>longName</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>comparer</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.stringcomparer" target="_blank">System.StringComparer</a><br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">Boolean</a>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>. When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Core_NameExtensions">NameExtensions Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />