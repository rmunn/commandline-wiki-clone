# ParserSettings.ParsingCulture Property 
 

Gets or sets the culture used when parsing arguments to typed properties.

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public CultureInfo ParsingCulture { get; set; }
```

**VB**<br />
``` VB
Public Property ParsingCulture As CultureInfo
	Get
	Set
```

**C++**<br />
``` C++
public:
property CultureInfo^ ParsingCulture {
	CultureInfo^ get ();
	void set (CultureInfo^ value);
}
```

**F#**<br />
``` F#
member ParsingCulture : CultureInfo with get, set

```


#### Property Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.globalization.cultureinfo" target="_blank">CultureInfo</a>

## Remarks
Default is invariant culture, <a href="https://docs.microsoft.com/dotnet/api/system.globalization.cultureinfo.invariantculture#System_Globalization_CultureInfo_InvariantCulture" target="_blank">InvariantCulture</a>.

## See Also


#### Reference
<a href="T_CommandLine_ParserSettings">ParserSettings Class</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />