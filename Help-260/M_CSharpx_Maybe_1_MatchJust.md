# Maybe(*T*).MatchJust Method 
 

Matches a value returning `true` and value itself via output parameter.

**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public bool MatchJust(
	out T value
)
```

**VB**<br />
``` VB
Public Function MatchJust ( 
	<OutAttribute> ByRef value As T
) As Boolean
```

**C++**<br />
``` C++
public:
bool MatchJust(
	[OutAttribute] T% value
)
```

**F#**<br />
``` F#
member MatchJust : 
        value : 'T byref -> bool 

```


#### Parameters
&nbsp;<dl><dt>value</dt><dd>Type: <a href="T_CSharpx_Maybe_1">*T*</a><br /></dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">Boolean</a>

## See Also


#### Reference
<a href="T_CSharpx_Maybe_1">Maybe(T) Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />