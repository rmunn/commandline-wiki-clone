# InstanceChooser.MakeNotParsed Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static NotParsed<Object> MakeNotParsed(
	IEnumerable<Type> types,
	params Error[] errors
)
```

**VB**<br />
``` VB
Private Shared Function MakeNotParsed ( 
	types As IEnumerable(Of Type),
	ParamArray errors As Error()
) As NotParsed(Of Object)
```

**C++**<br />
``` C++
private:
static NotParsed<Object^>^ MakeNotParsed(
	IEnumerable<Type^>^ types, 
	... array<Error^>^ errors
)
```

**F#**<br />
``` F#
private static member MakeNotParsed : 
        types : IEnumerable<Type> * 
        errors : Error[] -> NotParsed<Object> 

```


#### Parameters
&nbsp;<dl><dt>types</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a>)<br /></dd><dt>errors</dt><dd>Type: <a href="T_CommandLine_Error">CommandLine.Error</a>[]<br /></dd></dl>

#### Return Value
Type: <a href="T_CommandLine_NotParsed_1">NotParsed</a>(<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>)

## See Also


#### Reference
<a href="T_CommandLine_Core_InstanceChooser">InstanceChooser Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />