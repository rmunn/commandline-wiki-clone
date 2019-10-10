# ParserSettings.HelpWriter Property 
 

Gets or sets the <a href="https://docs.microsoft.com/dotnet/api/system.io.textwriter" target="_blank">TextWriter</a> used for help method output. Setting this property to null, will disable help screen.

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public TextWriter HelpWriter { get; set; }
```

**VB**<br />
``` VB
Public Property HelpWriter As TextWriter
	Get
	Set
```

**C++**<br />
``` C++
public:
property TextWriter^ HelpWriter {
	TextWriter^ get ();
	void set (TextWriter^ value);
}
```

**F#**<br />
``` F#
member HelpWriter : TextWriter with get, set

```


#### Property Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.io.textwriter" target="_blank">TextWriter</a>

## Remarks
It is the caller's responsibility to dispose or close the <a href="https://docs.microsoft.com/dotnet/api/system.io.textwriter" target="_blank">TextWriter</a>.

## See Also


#### Reference
<a href="T_CommandLine_ParserSettings">ParserSettings Class</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />