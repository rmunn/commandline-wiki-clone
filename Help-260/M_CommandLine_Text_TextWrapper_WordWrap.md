# TextWrapper.WordWrap Method 
 

Splits a string into a words and performs wrapping while also preserving line-breaks and sub-indentation

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public TextWrapper WordWrap(
	int columnWidth
)
```

**VB**<br />
``` VB
Public Function WordWrap ( 
	columnWidth As Integer
) As TextWrapper
```

**C++**<br />
``` C++
public:
TextWrapper^ WordWrap(
	int columnWidth
)
```

**F#**<br />
``` F#
member WordWrap : 
        columnWidth : int -> TextWrapper 

```


#### Parameters
&nbsp;<dl><dt>columnWidth</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">System.Int32</a><br />The number of characters we can use for text</dd></dl>

#### Return Value
Type: <a href="T_CommandLine_Text_TextWrapper">TextWrapper</a><br />this

## Remarks
This method attempts to wrap text without breaking words For example, if columnWidth is 10 , the input "a string for wrapping 01234567890123" would return "a string "for "wrapping "0123456789 "0123"

## See Also


#### Reference
<a href="T_CommandLine_Text_TextWrapper">TextWrapper Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />