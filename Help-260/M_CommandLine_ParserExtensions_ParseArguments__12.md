# ParserExtensions.ParseArguments(*T1*, *T2*, *T3*, *T4*, *T5*, *T6*, *T7*, *T8*, *T9*, *T10*, *T11*, *T12*) Method (Parser, IEnumerable(String))
 

Parses a string array of command line arguments for verb commands scenario, constructing the proper instance from types as generic arguments. Grammar rules are defined decorating public properties with appropriate attributes. The <a href="T_CommandLine_VerbAttribute">VerbAttribute</a> must be applied to types in the array.

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static ParserResult<Object> ParseArguments<T1, T2, T3, T4, T5, T6, T7, T8, T9, T10, T11, T12>(
	this Parser parser,
	IEnumerable<string> args
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function ParseArguments(Of T1, T2, T3, T4, T5, T6, T7, T8, T9, T10, T11, T12) ( 
	parser As Parser,
	args As IEnumerable(Of String)
) As ParserResult(Of Object)
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T1, typename T2, typename T3, typename T4, typename T5, typename T6, typename T7, typename T8, typename T9, typename T10, typename T11, typename T12>
static ParserResult<Object^>^ ParseArguments(
	Parser^ parser, 
	IEnumerable<String^>^ args
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member ParseArguments : 
        parser : Parser * 
        args : IEnumerable<string> -> ParserResult<Object> 

```


#### Parameters
&nbsp;<dl><dt>parser</dt><dd>Type: <a href="T_CommandLine_Parser">CommandLine.Parser</a><br />A <a href="T_CommandLine_Parser">Parser</a> instance.</dd><dt>args</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)<br />A <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a> array of command line arguments, normally supplied by application entry point.</dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T1</dt><dd>The type of the first verb.</dd><dt>T2</dt><dd>The type of the second verb.</dd><dt>T3</dt><dd>The type of the third verb.</dd><dt>T4</dt><dd>The type of the fourth verb.</dd><dt>T5</dt><dd>The type of the fifth verb.</dd><dt>T6</dt><dd>The type of the sixth verb.</dd><dt>T7</dt><dd>The type of the seventh verb.</dd><dt>T8</dt><dd>The type of the eighth verb.</dd><dt>T9</dt><dd>The type of the ninth verb.</dd><dt>T10</dt><dd>The type of the tenth verb.</dd><dt>T11</dt><dd>The type of the eleventh verb.</dd><dt>T12</dt><dd>The type of the twelfth verb.</dd></dl>

#### Return Value
Type: <a href="T_CommandLine_ParserResult_1">ParserResult</a>(<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>)<br />A <a href="T_CommandLine_ParserResult_1">ParserResult(T)</a> containing the appropriate instance with parsed values as a <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a> and a sequence of <a href="T_CommandLine_Error">Error</a>.

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CommandLine_Parser">Parser</a>. When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## Exceptions
&nbsp;<table><tr><th>Exception</th><th>Condition</th></tr><tr><td><a href="https://docs.microsoft.com/dotnet/api/system.argumentnullexception" target="_blank">ArgumentNullException</a></td><td>Thrown if one or more arguments are null.</td></tr></table>

## Remarks
All types must expose a parameterless constructor.

## See Also


#### Reference
<a href="T_CommandLine_ParserExtensions">ParserExtensions Class</a><br /><a href="Overload_CommandLine_ParserExtensions_ParseArguments">ParseArguments Overload</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />