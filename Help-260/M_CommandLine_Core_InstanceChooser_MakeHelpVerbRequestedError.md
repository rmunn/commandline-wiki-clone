# InstanceChooser.MakeHelpVerbRequestedError Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static HelpVerbRequestedError MakeHelpVerbRequestedError(
	IEnumerable<Tuple<Verb, Type>> verbs,
	string verb,
	StringComparer nameComparer
)
```

**VB**<br />
``` VB
Private Shared Function MakeHelpVerbRequestedError ( 
	verbs As IEnumerable(Of Tuple(Of Verb, Type)),
	verb As String,
	nameComparer As StringComparer
) As HelpVerbRequestedError
```

**C++**<br />
``` C++
private:
static HelpVerbRequestedError^ MakeHelpVerbRequestedError(
	IEnumerable<Tuple<Verb^, Type^>^>^ verbs, 
	String^ verb, 
	StringComparer^ nameComparer
)
```

**F#**<br />
``` F#
private static member MakeHelpVerbRequestedError : 
        verbs : IEnumerable<Tuple<Verb, Type>> * 
        verb : string * 
        nameComparer : StringComparer -> HelpVerbRequestedError 

```


#### Parameters
&nbsp;<dl><dt>verbs</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.tuple-2" target="_blank">Tuple</a>(<a href="T_CommandLine_Core_Verb">Verb</a>, <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a>))<br /></dd><dt>verb</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>nameComparer</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.stringcomparer" target="_blank">System.StringComparer</a><br /></dd></dl>

#### Return Value
Type: <a href="T_CommandLine_HelpVerbRequestedError">HelpVerbRequestedError</a>

## See Also


#### Reference
<a href="T_CommandLine_Core_InstanceChooser">InstanceChooser Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />