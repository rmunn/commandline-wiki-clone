# TypeDescriptor.Create Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static TypeDescriptor Create(
	TargetType tag,
	Maybe<int> maximumItems,
	TypeDescriptor next = null
)
```

**VB**<br />
``` VB
Public Shared Function Create ( 
	tag As TargetType,
	maximumItems As Maybe(Of Integer),
	Optional next As TypeDescriptor = Nothing
) As TypeDescriptor
```

**C++**<br />
``` C++
public:
static TypeDescriptor Create(
	TargetType tag, 
	Maybe<int>^ maximumItems, 
	TypeDescriptor next = nullptr
)
```

**F#**<br />
``` F#
static member Create : 
        tag : TargetType * 
        maximumItems : Maybe<int> * 
        ?next : TypeDescriptor 
(* Defaults:
        let _next = defaultArg next null
*)
-> TypeDescriptor 

```


#### Parameters
&nbsp;<dl><dt>tag</dt><dd>Type: <a href="T_CommandLine_Core_TargetType">CommandLine.Core.TargetType</a><br /></dd><dt>maximumItems</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">Int32</a>)<br /></dd><dt>next (Optional)</dt><dd>Type: <a href="T_CommandLine_Core_TypeDescriptor">CommandLine.Core.TypeDescriptor</a><br /></dd></dl>

#### Return Value
Type: <a href="T_CommandLine_Core_TypeDescriptor">TypeDescriptor</a>

## See Also


#### Reference
<a href="T_CommandLine_Core_TypeDescriptor">TypeDescriptor Structure</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />