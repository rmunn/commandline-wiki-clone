# HeadingInfo.Default Property 
 

Gets the default heading instance. The title is retrieved from <a href="https://docs.microsoft.com/dotnet/api/system.reflection.assemblytitleattribute" target="_blank">AssemblyTitleAttribute</a>, or the assembly short name if its not defined. The version is retrieved from <a href="https://docs.microsoft.com/dotnet/api/system.reflection.assemblyinformationalversionattribute" target="_blank">AssemblyInformationalVersionAttribute</a>, or the assembly version if its not defined.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static HeadingInfo Default { get; }
```

**VB**<br />
``` VB
Public Shared ReadOnly Property Default As HeadingInfo
	Get
```

**C++**<br />
``` C++
public:
static property HeadingInfo^ Default {
	HeadingInfo^ get ();
}
```

**F#**<br />
``` F#
static member Default : HeadingInfo with get

```


#### Property Value
Type: <a href="T_CommandLine_Text_HeadingInfo">HeadingInfo</a>

## See Also


#### Reference
<a href="T_CommandLine_Text_HeadingInfo">HeadingInfo Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />