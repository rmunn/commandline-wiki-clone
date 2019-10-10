# ParserSettings.IgnoreUnknownArguments Property 
 

Gets or sets a value indicating whether the parser shall move on to the next argument and ignore the given argument if it encounter an unknown arguments

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public bool IgnoreUnknownArguments { get; set; }
```

**VB**<br />
``` VB
Public Property IgnoreUnknownArguments As Boolean
	Get
	Set
```

**C++**<br />
``` C++
public:
property bool IgnoreUnknownArguments {
	bool get ();
	void set (bool value);
}
```

**F#**<br />
``` F#
member IgnoreUnknownArguments : bool with get, set

```


#### Property Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">Boolean</a><br />`true` to allow parsing the arguments with different class options that do not have all the arguments.

## Remarks
This allows fragmented version class parsing, useful for project with add-on where add-ons also requires command line arguments but when these are unknown by the main program at build time.

## See Also


#### Reference
<a href="T_CommandLine_ParserSettings">ParserSettings Class</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />