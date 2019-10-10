# VerbAttribute Constructor 
 

Initializes a new instance of the <a href="T_CommandLine_VerbAttribute">VerbAttribute</a> class.

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public VerbAttribute(
	string name
)
```

**VB**<br />
``` VB
Public Sub New ( 
	name As String
)
```

**C++**<br />
``` C++
public:
VerbAttribute(
	String^ name
)
```

**F#**<br />
``` F#
new : 
        name : string -> VerbAttribute
```


#### Parameters
&nbsp;<dl><dt>name</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br />The long name of the verb command.</dd></dl>

## Exceptions
&nbsp;<table><tr><th>Exception</th><th>Condition</th></tr><tr><td><a href="https://docs.microsoft.com/dotnet/api/system.argumentexception" target="_blank">ArgumentException</a></td><td>Thrown if *name* is null, empty or whitespace.</td></tr></table>

## See Also


#### Reference
<a href="T_CommandLine_VerbAttribute">VerbAttribute Class</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />