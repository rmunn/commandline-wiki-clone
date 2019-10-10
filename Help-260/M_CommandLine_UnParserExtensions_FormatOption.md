# UnParserExtensions.FormatOption Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static string FormatOption(
	OptionSpecification spec,
	Object value,
	UnParserSettings settings
)
```

**VB**<br />
``` VB
Private Shared Function FormatOption ( 
	spec As OptionSpecification,
	value As Object,
	settings As UnParserSettings
) As String
```

**C++**<br />
``` C++
private:
static String^ FormatOption(
	OptionSpecification^ spec, 
	Object^ value, 
	UnParserSettings^ settings
)
```

**F#**<br />
``` F#
private static member FormatOption : 
        spec : OptionSpecification * 
        value : Object * 
        settings : UnParserSettings -> string 

```


#### Parameters
&nbsp;<dl><dt>spec</dt><dd>Type: <a href="T_CommandLine_Core_OptionSpecification">CommandLine.Core.OptionSpecification</a><br /></dd><dt>value</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br /></dd><dt>settings</dt><dd>Type: <a href="T_CommandLine_UnParserSettings">CommandLine.UnParserSettings</a><br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>

## See Also


#### Reference
<a href="T_CommandLine_UnParserExtensions">UnParserExtensions Class</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />