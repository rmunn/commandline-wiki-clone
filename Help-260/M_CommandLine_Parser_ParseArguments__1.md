# Parser.ParseArguments(*T*) Method (IEnumerable(String))
 

Parses a string array of command line arguments constructing values in an instance of type *T*. Grammar rules are defined decorating public properties with appropriate attributes.

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public ParserResult<T> ParseArguments<T>(
	IEnumerable<string> args
)

```

**VB**<br />
``` VB
Public Function ParseArguments(Of T) ( 
	args As IEnumerable(Of String)
) As ParserResult(Of T)
```

**C++**<br />
``` C++
public:
generic<typename T>
ParserResult<T>^ ParseArguments(
	IEnumerable<String^>^ args
)
```

**F#**<br />
``` F#
member ParseArguments : 
        args : IEnumerable<string> -> ParserResult<'T> 

```


#### Parameters
&nbsp;<dl><dt>args</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)<br />A <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a> array of command line arguments, normally supplied by application entry point.</dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd>Type of the target instance built with parsed value.</dd></dl>

#### Return Value
Type: <a href="T_CommandLine_ParserResult_1">ParserResult</a>(*T*)<br />A <a href="T_CommandLine_ParserResult_1">ParserResult(T)</a> containing an instance of type *T* with parsed values and a sequence of <a href="T_CommandLine_Error">Error</a>.

## Exceptions
&nbsp;<table><tr><th>Exception</th><th>Condition</th></tr><tr><td><a href="https://docs.microsoft.com/dotnet/api/system.argumentnullexception" target="_blank">ArgumentNullException</a></td><td>Thrown if one or more arguments are null.</td></tr></table>

## See Also


#### Reference
<a href="T_CommandLine_Parser">Parser Class</a><br /><a href="Overload_CommandLine_Parser_ParseArguments">ParseArguments Overload</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />