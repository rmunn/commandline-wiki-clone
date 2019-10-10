# UnParserExtensions.FormatName Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static string FormatName(
	this OptionSpecification optionSpec,
	UnParserSettings settings
)
```

**VB**<br />
``` VB
<ExtensionAttribute>
Private Shared Function FormatName ( 
	optionSpec As OptionSpecification,
	settings As UnParserSettings
) As String
```

**C++**<br />
``` C++
private:
[ExtensionAttribute]
static String^ FormatName(
	OptionSpecification^ optionSpec, 
	UnParserSettings^ settings
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
private static member FormatName : 
        optionSpec : OptionSpecification * 
        settings : UnParserSettings -> string 

```


#### Parameters
&nbsp;<dl><dt>optionSpec</dt><dd>Type: <a href="T_CommandLine_Core_OptionSpecification">CommandLine.Core.OptionSpecification</a><br /></dd><dt>settings</dt><dd>Type: <a href="T_CommandLine_UnParserSettings">CommandLine.UnParserSettings</a><br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CommandLine_Core_OptionSpecification">OptionSpecification</a>. When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_UnParserExtensions">UnParserExtensions Class</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />