# OptionSpecification.NewSwitch Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static OptionSpecification NewSwitch(
	string shortName,
	string longName,
	bool required,
	string helpText,
	string metaValue,
	bool hidden = false
)
```

**VB**<br />
``` VB
Public Shared Function NewSwitch ( 
	shortName As String,
	longName As String,
	required As Boolean,
	helpText As String,
	metaValue As String,
	Optional hidden As Boolean = false
) As OptionSpecification
```

**C++**<br />
``` C++
public:
static OptionSpecification^ NewSwitch(
	String^ shortName, 
	String^ longName, 
	bool required, 
	String^ helpText, 
	String^ metaValue, 
	bool hidden = false
)
```

**F#**<br />
``` F#
static member NewSwitch : 
        shortName : string * 
        longName : string * 
        required : bool * 
        helpText : string * 
        metaValue : string * 
        ?hidden : bool 
(* Defaults:
        let _hidden = defaultArg hidden false
*)
-> OptionSpecification 

```


#### Parameters
&nbsp;<dl><dt>shortName</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>longName</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>required</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br /></dd><dt>helpText</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>metaValue</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>hidden (Optional)</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br /></dd></dl>

#### Return Value
Type: <a href="T_CommandLine_Core_OptionSpecification">OptionSpecification</a>

## See Also


#### Reference
<a href="T_CommandLine_Core_OptionSpecification">OptionSpecification Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />