# Parser.ParseArguments Method (IEnumerable(String), Type[])
 

Parses a string array of command line arguments for verb commands scenario, constructing the proper instance from the array of types supplied by *types*. Grammar rules are defined decorating public properties with appropriate attributes. The <a href="T_CommandLine_VerbAttribute">VerbAttribute</a> must be applied to types in the array.

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public ParserResult<Object> ParseArguments(
	IEnumerable<string> args,
	params Type[] types
)
```

**VB**<br />
``` VB
Public Function ParseArguments ( 
	args As IEnumerable(Of String),
	ParamArray types As Type()
) As ParserResult(Of Object)
```

**C++**<br />
``` C++
public:
ParserResult<Object^>^ ParseArguments(
	IEnumerable<String^>^ args, 
	... array<Type^>^ types
)
```

**F#**<br />
``` F#
member ParseArguments : 
        args : IEnumerable<string> * 
        types : Type[] -> ParserResult<Object> 

```


#### Parameters
&nbsp;<dl><dt>args</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)<br />A <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a> array of command line arguments, normally supplied by application entry point.</dd><dt>types</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">System.Type</a>[]<br />A <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a> array used to supply verb alternatives.</dd></dl>

#### Return Value
Type: <a href="T_CommandLine_ParserResult_1">ParserResult</a>(<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>)<br />A <a href="T_CommandLine_ParserResult_1">ParserResult(T)</a> containing the appropriate instance with parsed values as a <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a> and a sequence of <a href="T_CommandLine_Error">Error</a>.

## Exceptions
&nbsp;<table><tr><th>Exception</th><th>Condition</th></tr><tr><td><a href="https://docs.microsoft.com/dotnet/api/system.argumentnullexception" target="_blank">ArgumentNullException</a></td><td>Thrown if one or more arguments are null.</td></tr><tr><td><a href="https://docs.microsoft.com/dotnet/api/system.argumentoutofrangeexception" target="_blank">ArgumentOutOfRangeException</a></td><td>Thrown if *types* array is empty.</td></tr></table>

## Remarks
All types must expose a parameterless constructor. It's strongly recommended to use a generic overload.

## See Also


#### Reference
<a href="T_CommandLine_Parser">Parser Class</a><br /><a href="Overload_CommandLine_Parser_ParseArguments">ParseArguments Overload</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />