# Verb Constructor 
 

Initializes a new instance of the <a href="T_CommandLine_Core_Verb">Verb</a> class

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public Verb(
	string name,
	string helpText,
	bool hidden = false
)
```

**VB**<br />
``` VB
Public Sub New ( 
	name As String,
	helpText As String,
	Optional hidden As Boolean = false
)
```

**C++**<br />
``` C++
public:
Verb(
	String^ name, 
	String^ helpText, 
	bool hidden = false
)
```

**F#**<br />
``` F#
new : 
        name : string * 
        helpText : string * 
        ?hidden : bool 
(* Defaults:
        let _hidden = defaultArg hidden false
*)
-> Verb
```


#### Parameters
&nbsp;<dl><dt>name</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>helpText</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>hidden (Optional)</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br /></dd></dl>

## See Also


#### Reference
<a href="T_CommandLine_Core_Verb">Verb Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />