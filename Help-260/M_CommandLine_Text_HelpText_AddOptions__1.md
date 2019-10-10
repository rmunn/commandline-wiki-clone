# HelpText.AddOptions(*T*) Method (ParserResult(*T*))
 

Adds a text block with options usage string.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public HelpText AddOptions<T>(
	ParserResult<T> result
)

```

**VB**<br />
``` VB
Public Function AddOptions(Of T) ( 
	result As ParserResult(Of T)
) As HelpText
```

**C++**<br />
``` C++
public:
generic<typename T>
HelpText^ AddOptions(
	ParserResult<T>^ result
)
```

**F#**<br />
``` F#
member AddOptions : 
        result : ParserResult<'T> -> HelpText 

```


#### Parameters
&nbsp;<dl><dt>result</dt><dd>Type: <a href="T_CommandLine_ParserResult_1">CommandLine.ParserResult</a>(*T*)<br />A parsing computation result.</dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: <a href="T_CommandLine_Text_HelpText">HelpText</a>

## Exceptions
&nbsp;<table><tr><th>Exception</th><th>Condition</th></tr><tr><td><a href="https://docs.microsoft.com/dotnet/api/system.argumentnullexception" target="_blank">ArgumentNullException</a></td><td>Thrown when parameter *result* is null.</td></tr></table>

## See Also


#### Reference
<a href="T_CommandLine_Text_HelpText">HelpText Class</a><br /><a href="Overload_CommandLine_Text_HelpText_AddOptions">AddOptions Overload</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />