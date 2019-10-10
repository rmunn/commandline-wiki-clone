# TokenError Constructor 
 

Initializes a new instance of the <a href="T_CommandLine_TokenError">TokenError</a> class.

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
protected TokenError(
	ErrorType tag,
	string token
)
```

**VB**<br />
``` VB
Protected Sub New ( 
	tag As ErrorType,
	token As String
)
```

**C++**<br />
``` C++
protected:
TokenError(
	ErrorType tag, 
	String^ token
)
```

**F#**<br />
``` F#
new : 
        tag : ErrorType * 
        token : string -> TokenError
```


#### Parameters
&nbsp;<dl><dt>tag</dt><dd>Type: <a href="T_CommandLine_ErrorType">CommandLine.ErrorType</a><br />Error type.</dd><dt>token</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br />Problematic token.</dd></dl>

## See Also


#### Reference
<a href="T_CommandLine_TokenError">TokenError Class</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />