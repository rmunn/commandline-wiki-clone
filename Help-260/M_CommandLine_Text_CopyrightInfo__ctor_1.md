# CopyrightInfo Constructor (Boolean, String, Int32[])
 

Initializes a new instance of the <a href="T_CommandLine_Text_CopyrightInfo">CopyrightInfo</a> class specifying symbol case, author and copyrightYears.

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public CopyrightInfo(
	bool isSymbolUpper,
	string author,
	params int[] copyrightYears
)
```

**VB**<br />
``` VB
Public Sub New ( 
	isSymbolUpper As Boolean,
	author As String,
	ParamArray copyrightYears As Integer()
)
```

**C++**<br />
``` C++
public:
CopyrightInfo(
	bool isSymbolUpper, 
	String^ author, 
	... array<int>^ copyrightYears
)
```

**F#**<br />
``` F#
new : 
        isSymbolUpper : bool * 
        author : string * 
        copyrightYears : int[] -> CopyrightInfo
```


#### Parameters
&nbsp;<dl><dt>isSymbolUpper</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br />The case of the copyright symbol.</dd><dt>author</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br />The company or person holding the copyright.</dd><dt>copyrightYears</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">System.Int32</a>[]<br />The copyrightYears of coverage of copyright.</dd></dl>

## Exceptions
&nbsp;<table><tr><th>Exception</th><th>Condition</th></tr><tr><td><a href="https://docs.microsoft.com/dotnet/api/system.argumentexception" target="_blank">ArgumentException</a></td><td>Thrown when parameter *author* is null or empty string.</td></tr><tr><td><a href="https://docs.microsoft.com/dotnet/api/system.argumentoutofrangeexception" target="_blank">ArgumentOutOfRangeException</a></td><td>Thrown when parameter *copyrightYears* is not supplied.</td></tr></table>

## See Also


#### Reference
<a href="T_CommandLine_Text_CopyrightInfo">CopyrightInfo Class</a><br /><a href="Overload_CommandLine_Text_CopyrightInfo__ctor">CopyrightInfo Overload</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />