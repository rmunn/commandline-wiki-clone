# StringBuilderExtensions.TrimEndIfMatchWhen Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Infrastructure">CommandLine.Infrastructure</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static StringBuilder TrimEndIfMatchWhen(
	this StringBuilder builder,
	bool condition,
	char c
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function TrimEndIfMatchWhen ( 
	builder As StringBuilder,
	condition As Boolean,
	c As Char
) As StringBuilder
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
static StringBuilder^ TrimEndIfMatchWhen(
	StringBuilder^ builder, 
	bool condition, 
	wchar_t c
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member TrimEndIfMatchWhen : 
        builder : StringBuilder * 
        condition : bool * 
        c : char -> StringBuilder 

```


#### Parameters
&nbsp;<dl><dt>builder</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.text.stringbuilder" target="_blank">System.Text.StringBuilder</a><br /></dd><dt>condition</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br /></dd><dt>c</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.char" target="_blank">System.Char</a><br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.text.stringbuilder" target="_blank">StringBuilder</a>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.text.stringbuilder" target="_blank">StringBuilder</a>. When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Infrastructure_StringBuilderExtensions">StringBuilderExtensions Class</a><br /><a href="N_CommandLine_Infrastructure">CommandLine.Infrastructure Namespace</a><br />