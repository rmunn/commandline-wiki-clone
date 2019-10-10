# MultilineTextAttribute.AddToHelpText Method (HelpText, Func(String, HelpText))
 

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
internal HelpText AddToHelpText(
	HelpText helpText,
	Func<string, HelpText> func
)
```

**VB**<br />
``` VB
Friend Function AddToHelpText ( 
	helpText As HelpText,
	func As Func(Of String, HelpText)
) As HelpText
```

**C++**<br />
``` C++
internal:
HelpText^ AddToHelpText(
	HelpText^ helpText, 
	Func<String^, HelpText^>^ func
)
```

**F#**<br />
``` F#
internal member AddToHelpText : 
        helpText : HelpText * 
        func : Func<string, HelpText> -> HelpText 

```


#### Parameters
&nbsp;<dl><dt>helpText</dt><dd>Type: <a href="T_CommandLine_Text_HelpText">CommandLine.Text.HelpText</a><br /></dd><dt>func</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.func-2" target="_blank">System.Func</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>, <a href="T_CommandLine_Text_HelpText">HelpText</a>)<br /></dd></dl>

#### Return Value
Type: <a href="T_CommandLine_Text_HelpText">HelpText</a>

## See Also


#### Reference
<a href="T_CommandLine_Text_MultilineTextAttribute">MultilineTextAttribute Class</a><br /><a href="Overload_CommandLine_Text_MultilineTextAttribute_AddToHelpText">AddToHelpText Overload</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />