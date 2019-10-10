# UnParserExtensions.FormatCommandLine(*T*) Method (Parser, *T*, Action(UnParserSettings))
 

Format a command line argument string from a parsed instance.

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static string FormatCommandLine<T>(
	this Parser parser,
	T options,
	Action<UnParserSettings> configuration
)

```

**VB**<br />
``` VB
<ExtensionAttribute>
Public Shared Function FormatCommandLine(Of T) ( 
	parser As Parser,
	options As T,
	configuration As Action(Of UnParserSettings)
) As String
```

**C++**<br />
``` C++
public:
[ExtensionAttribute]
generic<typename T>
static String^ FormatCommandLine(
	Parser^ parser, 
	T options, 
	Action<UnParserSettings^>^ configuration
)
```

**F#**<br />
``` F#
[<ExtensionAttribute>]
static member FormatCommandLine : 
        parser : Parser * 
        options : 'T * 
        configuration : Action<UnParserSettings> -> string 

```


#### Parameters
&nbsp;<dl><dt>parser</dt><dd>Type: <a href="T_CommandLine_Parser">CommandLine.Parser</a><br />Parser instance.</dd><dt>options</dt><dd>Type: *T*<br />A parsed (or manually correctly constructed instance).</dd><dt>configuration</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.action-1" target="_blank">System.Action</a>(<a href="T_CommandLine_UnParserSettings">UnParserSettings</a>)<br />The <a href="https://docs.microsoft.com/dotnet/api/system.action-1" target="_blank">Action(T)</a> lambda used to configure aspects and behaviors of the unparsersing process.</dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd>Type of *options*.</dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a><br />A string with command line arguments.

#### Usage Note
In Visual Basic and C#, you can call this method as an instance method on any object of type <a href="T_CommandLine_Parser">Parser</a>. When you use instance method syntax to call this method, omit the first parameter. For more information, see <a href="https://docs.microsoft.com/dotnet/visual-basic/programming-guide/language-features/procedures/extension-methods">Extension Methods (Visual Basic)</a> or <a href="https://docs.microsoft.com/dotnet/csharp/programming-guide/classes-and-structs/extension-methods">Extension Methods (C# Programming Guide)</a>.

## See Also


#### Reference
<a href="T_CommandLine_UnParserExtensions">UnParserExtensions Class</a><br /><a href="Overload_CommandLine_UnParserExtensions_FormatCommandLine">FormatCommandLine Overload</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />