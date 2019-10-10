# NamedError Constructor 
 

Initializes a new instance of the <a href="T_CommandLine_NamedError">NamedError</a> class.

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
protected NamedError(
	ErrorType tag,
	NameInfo nameInfo
)
```

**VB**<br />
``` VB
Protected Sub New ( 
	tag As ErrorType,
	nameInfo As NameInfo
)
```

**C++**<br />
``` C++
protected:
NamedError(
	ErrorType tag, 
	NameInfo^ nameInfo
)
```

**F#**<br />
``` F#
new : 
        tag : ErrorType * 
        nameInfo : NameInfo -> NamedError
```


#### Parameters
&nbsp;<dl><dt>tag</dt><dd>Type: <a href="T_CommandLine_ErrorType">CommandLine.ErrorType</a><br />Error type.</dd><dt>nameInfo</dt><dd>Type: <a href="T_CommandLine_NameInfo">CommandLine.NameInfo</a><br />Problematic name.</dd></dl>

## See Also


#### Reference
<a href="T_CommandLine_NamedError">NamedError Class</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />