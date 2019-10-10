# TextWrapper.WrapAndIndentText Method 
 

Convenience method to wraps and indent a string in a single operation

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static string WrapAndIndentText(
	string input,
	int indentLevel,
	int columnWidth
)
```

**VB**<br />
``` VB
Public Shared Function WrapAndIndentText ( 
	input As String,
	indentLevel As Integer,
	columnWidth As Integer
) As String
```

**C++**<br />
``` C++
public:
static String^ WrapAndIndentText(
	String^ input, 
	int indentLevel, 
	int columnWidth
)
```

**F#**<br />
``` F#
static member WrapAndIndentText : 
        input : string * 
        indentLevel : int * 
        columnWidth : int -> string 

```


#### Parameters
&nbsp;<dl><dt>input</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br />The string to operate on</dd><dt>indentLevel</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">System.Int32</a><br />The number of spaces to indent by</dd><dt>columnWidth</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">System.Int32</a><br />The width of the column used for wrapping</dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a><br />the processed string

## Remarks
The string is wrapped _then_ indented so the columnWidth is the width of the usable text block, and does NOT include the indentLevel.

## See Also


#### Reference
<a href="T_CommandLine_Text_TextWrapper">TextWrapper Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />