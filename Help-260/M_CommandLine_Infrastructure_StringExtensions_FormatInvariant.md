# StringExtensions.FormatInvariant Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Infrastructure">CommandLine.Infrastructure</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static string FormatInvariant(
	this string value,
	params Object[] arguments
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function FormatInvariant ( 
	value As String,
	ParamArray arguments As Object()
) As String
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
static String^ FormatInvariant(
	String^ value, 
	... array<Object^>^ arguments
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member FormatInvariant : 
        value : string * 
        arguments : Object[] -> string 

```


#### Parameters
&nbsp;<dl><dt>value</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>arguments</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a>[]<br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>. When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Infrastructure_StringExtensions">StringExtensions Class</a><br /><a href="N_CommandLine_Infrastructure">CommandLine.Infrastructure Namespace</a><br />