# HelpText.AddOptionsImpl Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private HelpText AddOptionsImpl(
	IEnumerable<Specification> specifications,
	string requiredWord,
	int maximumLength
)
```

**VB**<br />
``` VB
Private Function AddOptionsImpl ( 
	specifications As IEnumerable(Of Specification),
	requiredWord As String,
	maximumLength As Integer
) As HelpText
```

**C++**<br />
``` C++
private:
HelpText^ AddOptionsImpl(
	IEnumerable<Specification^>^ specifications, 
	String^ requiredWord, 
	int maximumLength
)
```

**F#**<br />
``` F#
private member AddOptionsImpl : 
        specifications : IEnumerable<Specification> * 
        requiredWord : string * 
        maximumLength : int -> HelpText 

```


#### Parameters
&nbsp;<dl><dt>specifications</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="T_CommandLine_Core_Specification">Specification</a>)<br /></dd><dt>requiredWord</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>maximumLength</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">System.Int32</a><br /></dd></dl>

#### Return Value
Type: <a href="T_CommandLine_Text_HelpText">HelpText</a>

## See Also


#### Reference
<a href="T_CommandLine_Text_HelpText">HelpText Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />