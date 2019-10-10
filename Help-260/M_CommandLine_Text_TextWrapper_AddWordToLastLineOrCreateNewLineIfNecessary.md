# TextWrapper.AddWordToLastLineOrCreateNewLineIfNecessary Method 
 

When presented with a word, either append to the last line in the list or start a new line

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static List<StringBuilder> AddWordToLastLineOrCreateNewLineIfNecessary(
	List<StringBuilder> lines,
	string word,
	int columnWidth
)
```

**VB**<br />
``` VB
Private Shared Function AddWordToLastLineOrCreateNewLineIfNecessary ( 
	lines As List(Of StringBuilder),
	word As String,
	columnWidth As Integer
) As List(Of StringBuilder)
```

**C++**<br />
``` C++
private:
static List<StringBuilder^>^ AddWordToLastLineOrCreateNewLineIfNecessary(
	List<StringBuilder^>^ lines, 
	String^ word, 
	int columnWidth
)
```

**F#**<br />
``` F#
private static member AddWordToLastLineOrCreateNewLineIfNecessary : 
        lines : List<StringBuilder> * 
        word : string * 
        columnWidth : int -> List<StringBuilder> 

```


#### Parameters
&nbsp;<dl><dt>lines</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.list-1" target="_blank">System.Collections.Generic.List</a>(<a href="https://docs.microsoft.com/dotnet/api/system.text.stringbuilder" target="_blank">StringBuilder</a>)<br />A list of StringBuilders containing results so far</dd><dt>word</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br />The individual word to append</dd><dt>columnWidth</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">System.Int32</a><br />The usable text space</dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.list-1" target="_blank">List</a>(<a href="https://docs.microsoft.com/dotnet/api/system.text.stringbuilder" target="_blank">StringBuilder</a>)<br />The same list as is passed in

## Remarks
The 'word' can actually be an empty string. It's important to keep these - empty strings allow us to preserve indentation and extra spaces within a line.

## See Also


#### Reference
<a href="T_CommandLine_Text_TextWrapper">TextWrapper Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />