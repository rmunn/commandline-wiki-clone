# HeadingInfo Constructor 
 

Initializes a new instance of the <a href="T_CommandLine_Text_HeadingInfo">HeadingInfo</a> class specifying program name and version.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public HeadingInfo(
	string programName,
	string version = null
)
```

**VB**<br />
``` VB
Public Sub New ( 
	programName As String,
	Optional version As String = Nothing
)
```

**C++**<br />
``` C++
public:
HeadingInfo(
	String^ programName, 
	String^ version = nullptr
)
```

**F#**<br />
``` F#
new : 
        programName : string * 
        ?version : string 
(* Defaults:
        let _version = defaultArg version null
*)
-> HeadingInfo
```


#### Parameters
&nbsp;<dl><dt>programName</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br />The name of the program.</dd><dt>version (Optional)</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br />The version of the program.</dd></dl>

## Exceptions
&nbsp;<table><tr><th>Exception</th><th>Condition</th></tr><tr><td><a href="https://docs.microsoft.com/dotnet/api/system.argumentexception" target="_blank">ArgumentException</a></td><td>Thrown when parameter *programName* is null or empty string.</td></tr></table>

## See Also


#### Reference
<a href="T_CommandLine_Text_HeadingInfo">HeadingInfo Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />