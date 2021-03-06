# HelpText.AddOption Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private HelpText AddOption(
	string requiredWord,
	int maxLength,
	Specification specification,
	int widthOfHelpText
)
```

**VB**<br />
``` VB
Private Function AddOption ( 
	requiredWord As String,
	maxLength As Integer,
	specification As Specification,
	widthOfHelpText As Integer
) As HelpText
```

**C++**<br />
``` C++
private:
HelpText^ AddOption(
	String^ requiredWord, 
	int maxLength, 
	Specification^ specification, 
	int widthOfHelpText
)
```

**F#**<br />
``` F#
private member AddOption : 
        requiredWord : string * 
        maxLength : int * 
        specification : Specification * 
        widthOfHelpText : int -> HelpText 

```


#### Parameters
&nbsp;<dl><dt>requiredWord</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>maxLength</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">System.Int32</a><br /></dd><dt>specification</dt><dd>Type: <a href="T_CommandLine_Core_Specification">CommandLine.Core.Specification</a><br /></dd><dt>widthOfHelpText</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">System.Int32</a><br /></dd></dl>

#### Return Value
Type: <a href="T_CommandLine_Text_HelpText">HelpText</a>

## See Also


#### Reference
<a href="T_CommandLine_Text_HelpText">HelpText Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />