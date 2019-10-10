# CopyrightInfo.Default Property 
 

Gets the default copyright information. Retrieved from <a href="https://docs.microsoft.com/dotnet/api/system.reflection.assemblycopyrightattribute" target="_blank">AssemblyCopyrightAttribute</a>, if it exists, otherwise it uses <a href="https://docs.microsoft.com/dotnet/api/system.reflection.assemblycompanyattribute" target="_blank">AssemblyCompanyAttribute</a> as copyright holder with the current year. If neither exists it throws an <a href="https://docs.microsoft.com/dotnet/api/system.invalidoperationexception" target="_blank">InvalidOperationException</a>.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static CopyrightInfo Default { get; }
```

**VB**<br />
``` VB
Public Shared ReadOnly Property Default As CopyrightInfo
	Get
```

**C++**<br />
``` C++
public:
static property CopyrightInfo^ Default {
	CopyrightInfo^ get ();
}
```

**F#**<br />
``` F#
static member Default : CopyrightInfo with get

```


#### Property Value
Type: <a href="T_CommandLine_Text_CopyrightInfo">CopyrightInfo</a>

## See Also


#### Reference
<a href="T_CommandLine_Text_CopyrightInfo">CopyrightInfo Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />