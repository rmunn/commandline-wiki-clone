# TypeDescriptor Constructor 
 

Initializes a new instance of the <a href="T_CommandLine_Core_TypeDescriptor">TypeDescriptor</a> class

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private TypeDescriptor(
	TargetType targetType,
	Maybe<int> maxItems,
	Maybe<TypeDescriptor> nextValue = null
)
```

**VB**<br />
``` VB
Private Sub New ( 
	targetType As TargetType,
	maxItems As Maybe(Of Integer),
	Optional nextValue As Maybe(Of TypeDescriptor) = Nothing
)
```

**C++**<br />
``` C++
private:
TypeDescriptor(
	TargetType targetType, 
	Maybe<int>^ maxItems, 
	Maybe<TypeDescriptor>^ nextValue = nullptr
)
```

**F#**<br />
``` F#
new : 
        targetType : TargetType * 
        maxItems : Maybe<int> * 
        ?nextValue : Maybe<TypeDescriptor> 
(* Defaults:
        let _nextValue = defaultArg nextValue null
*)
-> TypeDescriptor
```


#### Parameters
&nbsp;<dl><dt>targetType</dt><dd>Type: <a href="T_CommandLine_Core_TargetType">CommandLine.Core.TargetType</a><br /></dd><dt>maxItems</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">Int32</a>)<br /></dd><dt>nextValue (Optional)</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(<a href="T_CommandLine_Core_TypeDescriptor">TypeDescriptor</a>)<br /></dd></dl>

## See Also


#### Reference
<a href="T_CommandLine_Core_TypeDescriptor">TypeDescriptor Structure</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />