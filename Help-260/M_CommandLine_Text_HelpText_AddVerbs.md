# HelpText.AddVerbs Method (Int32, Type[])
 

Adds a text block with verbs usage string.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public HelpText AddVerbs(
	int maximumLength,
	params Type[] types
)
```

**VB**<br />
``` VB
Public Function AddVerbs ( 
	maximumLength As Integer,
	ParamArray types As Type()
) As HelpText
```

**C++**<br />
``` C++
public:
HelpText^ AddVerbs(
	int maximumLength, 
	... array<Type^>^ types
)
```

**F#**<br />
``` F#
member AddVerbs : 
        maximumLength : int * 
        types : Type[] -> HelpText 

```


#### Parameters
&nbsp;<dl><dt>maximumLength</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">System.Int32</a><br />The maximum length of the help screen.</dd><dt>types</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">System.Type</a>[]<br />The array of <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a> with verb commands.</dd></dl>

#### Return Value
Type: <a href="T_CommandLine_Text_HelpText">HelpText</a>

## Exceptions
&nbsp;<table><tr><th>Exception</th><th>Condition</th></tr><tr><td><a href="https://docs.microsoft.com/dotnet/api/system.argumentnullexception" target="_blank">ArgumentNullException</a></td><td>Thrown when parameter *types* is null.</td></tr><tr><td><a href="https://docs.microsoft.com/dotnet/api/system.argumentoutofrangeexception" target="_blank">ArgumentOutOfRangeException</a></td><td>Thrown if *types* array is empty.</td></tr></table>

## See Also


#### Reference
<a href="T_CommandLine_Text_HelpText">HelpText Class</a><br /><a href="Overload_CommandLine_Text_HelpText_AddVerbs">AddVerbs Overload</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />