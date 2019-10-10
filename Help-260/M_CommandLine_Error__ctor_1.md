# Error Constructor (ErrorType, Boolean)
 

Initializes a new instance of the <a href="T_CommandLine_Error">Error</a> class.

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
protected Error(
	ErrorType tag,
	bool stopsProcessing
)
```

**VB**<br />
``` VB
Protected Sub New ( 
	tag As ErrorType,
	stopsProcessing As Boolean
)
```

**C++**<br />
``` C++
protected:
Error(
	ErrorType tag, 
	bool stopsProcessing
)
```

**F#**<br />
``` F#
new : 
        tag : ErrorType * 
        stopsProcessing : bool -> Error
```


#### Parameters
&nbsp;<dl><dt>tag</dt><dd>Type: <a href="T_CommandLine_ErrorType">CommandLine.ErrorType</a><br />Type discriminator tag.</dd><dt>stopsProcessing</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br />Tells if error stops parsing process.</dd></dl>

## See Also


#### Reference
<a href="T_CommandLine_Error">Error Class</a><br /><a href="Overload_CommandLine_Error__ctor">Error Overload</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />