# OptionSpecification Constructor 
 

Initializes a new instance of the <a href="T_CommandLine_Core_OptionSpecification">OptionSpecification</a> class

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public OptionSpecification(
	string shortName,
	string longName,
	bool required,
	string setName,
	Maybe<int> min,
	Maybe<int> max,
	char separator,
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
	shortName As String,
	longName As String,
	required As Boolean,
	setName As String,
	min As Maybe(Of Integer),
	max As Maybe(Of Integer),
	separator As Char,
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
OptionSpecification(
	String^ shortName, 
	String^ longName, 
	bool required, 
	String^ setName, 
	Maybe<int>^ min, 
	Maybe<int>^ max, 
	wchar_t separator, 
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
        shortName : string * 
        longName : string * 
        required : bool * 
        setName : string * 
        min : Maybe<int> * 
        max : Maybe<int> * 
        separator : char * 
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
-> OptionSpecification
```


#### Parameters
&nbsp;<dl><dt>shortName</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>longName</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>required</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br /></dd><dt>setName</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>min</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">Int32</a>)<br /></dd><dt>max</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.int32" target="_blank">Int32</a>)<br /></dd><dt>separator</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.char" target="_blank">System.Char</a><br /></dd><dt>defaultValue</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>)<br /></dd><dt>helpText</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>metaValue</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">System.String</a><br /></dd><dt>enumValues</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>)<br /></dd><dt>conversionType</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">System.Type</a><br /></dd><dt>targetType</dt><dd>Type: <a href="T_CommandLine_Core_TargetType">CommandLine.Core.TargetType</a><br /></dd><dt>hidden (Optional)</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br /></dd></dl>

## See Also


#### Reference
<a href="T_CommandLine_Core_OptionSpecification">OptionSpecification Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />