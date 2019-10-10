# MultilineTextAttribute.GetLastLineWithText Method 
 

Returns the last line with text. Preserves blank lines if user intended by skipping a line.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
protected virtual int GetLastLineWithText(
	string[] value
)
```

**VB**<br />
``` VB
Protected Overridable Function GetLastLineWithText ( 
	value As String()
) As Integer
```

**C++**<br />
``` C++
protected:
virtual int GetLastLineWithText(
	array<String^>^ value
)
```

**F#**<br />
``` F#
abstract GetLastLineWithText : 
        value : string[] -> int 
override GetLastLineWithText : 
        value : string[] -> int 
```


#### Parameters
&nbsp;<dl><dt>value</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a>[]<br />The string array to process.</dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">Int32</a><br />The last index of line of the non-blank line.

## See Also


#### Reference
<a href="T_CommandLine_Text_MultilineTextAttribute">MultilineTextAttribute Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />