# ValueSpecification Constructor 
 

Initializes a new instance of the <a href="T_CommandLine_Core_ValueSpecification">ValueSpecification</a> class

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public ValueSpecification(
	int index,
	string metaName,
	bool required,
	Maybe<int> min,
	Maybe<int> max,
	Maybe<Object> defaultValue,
	string helpText,
	string metaValue,
	IEnumerable<string> enumValues,
	Type conversionType,
	TargetType targetType,
	bool hidden = false
)
```

**VB**<br />
``` VB
Public Sub New ( 
	index As Integer,
	metaName As String,
	required As Boolean,
	min As Maybe(Of Integer),
	max As Maybe(Of Integer),
	defaultValue As Maybe(Of Object),
	helpText As String,
	metaValue As String,
	enumValues As IEnumerable(Of String),
	conversionType As Type,
	targetType As TargetType,
	Optional hidden As Boolean = false
)
```

**C++**<br />
``` C++
public:
ValueSpecification(
	int index, 
	String^ metaName, 
	bool required, 
	Maybe<int>^ min, 
	Maybe<int>^ max, 
	Maybe<Object^>^ defaultValue, 
	String^ helpText, 
	String^ metaValue, 
	IEnumerable<String^>^ enumValues, 
	Type^ conversionType, 
	TargetType targetType, 
	bool hidden = false
)
```

**F#**<br />
``` F#
new : 
        index : int * 
        metaName : string * 
        required : bool * 
        min : Maybe<int> * 
        max : Maybe<int> * 
        defaultValue : Maybe<Object> * 
        helpText : string * 
        metaValue : string * 
        enumValues : IEnumerable<string> * 
        conversionType : Type * 
        targetType : TargetType * 
        ?hidden : bool 
(* Defaults:
        let _hidden = defaultArg hidden false
*)
-> ValueSpecification
```


#### Parameters
&nbsp;<dl><dt>index</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">System.Int32</a><br /></dd><dt>metaName</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>required</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br /></dd><dt>min</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">Int32</a>)<br /></dd><dt>max</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">Int32</a>)<br /></dd><dt>defaultValue</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>)<br /></dd><dt>helpText</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>metaValue</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>enumValues</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)<br /></dd><dt>conversionType</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">System.Type</a><br /></dd><dt>targetType</dt><dd>Type: <a href="T_CommandLine_Core_TargetType">CommandLine.Core.TargetType</a><br /></dd><dt>hidden (Optional)</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br /></dd></dl>

## See Also


#### Reference
<a href="T_CommandLine_Core_ValueSpecification">ValueSpecification Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />