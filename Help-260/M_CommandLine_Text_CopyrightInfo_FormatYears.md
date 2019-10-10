# CopyrightInfo.FormatYears Method 
 

When overridden in a derived class, allows to specify a new algorithm to render copyright copyrightYears as a <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a> instance.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
protected virtual string FormatYears(
	int[] years
)
```

**VB**<br />
``` VB
Protected Overridable Function FormatYears ( 
	years As Integer()
) As String
```

**C++**<br />
``` C++
protected:
virtual String^ FormatYears(
	array<int>^ years
)
```

**F#**<br />
``` F#
abstract FormatYears : 
        years : int[] -> string 
override FormatYears : 
        years : int[] -> string 
```


#### Parameters
&nbsp;<dl><dt>years</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">System.Int32</a>[]<br />A <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">Int32</a> array of copyrightYears.</dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a><br />A <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a> instance with copyright copyrightYears.

## See Also


#### Reference
<a href="T_CommandLine_Text_CopyrightInfo">CopyrightInfo Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />