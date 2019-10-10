# StringBuilderExtensions.AppendIf Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Infrastructure">CommandLine.Infrastructure</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static StringBuilder AppendIf(
	this StringBuilder builder,
	bool condition,
	string ifTrue,
	string ifFalse
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function AppendIf ( 
	builder As StringBuilder,
	condition As Boolean,
	ifTrue As String,
	ifFalse As String
) As StringBuilder
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
static StringBuilder^ AppendIf(
	StringBuilder^ builder, 
	bool condition, 
	String^ ifTrue, 
	String^ ifFalse
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member AppendIf : 
        builder : StringBuilder * 
        condition : bool * 
        ifTrue : string * 
        ifFalse : string -> StringBuilder 

```


#### Parameters
&nbsp;<dl><dt>builder</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.text.stringbuilder" target="_blank">System.Text.StringBuilder</a><br /></dd><dt>condition</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br /></dd><dt>ifTrue</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>ifFalse</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.text.stringbuilder" target="_blank">StringBuilder</a>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="https://docs.microsoft.com/dotnet/api/system.text.stringbuilder" target="_blank">StringBuilder</a>. When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_Infrastructure_StringBuilderExtensions">StringBuilderExtensions Class</a><br /><a href="N_CommandLine_Infrastructure">CommandLine.Infrastructure Namespace</a><br />