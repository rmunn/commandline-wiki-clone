# HelpText.GetUsageFromType Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static Maybe<Tuple<UsageAttribute, IEnumerable<Example>>> GetUsageFromType(
	Type type
)
```

**VB**<br />
``` VB
Private Shared Function GetUsageFromType ( 
	type As Type
) As Maybe(Of Tuple(Of UsageAttribute, IEnumerable(Of Example)))
```

**C++**<br />
``` C++
private:
static Maybe<Tuple<UsageAttribute^, IEnumerable<Example^>^>^>^ GetUsageFromType(
	Type^ type
)
```

**F#**<br />
``` F#
private static member GetUsageFromType : 
        type : Type -> Maybe<Tuple<UsageAttribute, IEnumerable<Example>>> 

```


#### Parameters
&nbsp;<dl><dt>type</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">System.Type</a><br /></dd></dl>

#### Return Value
Type: <a href="T_CSharpx_Maybe_1">Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.tuple-2" target="_blank">Tuple</a>(<a href="T_CommandLine_Text_UsageAttribute">UsageAttribute</a>, <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">IEnumerable</a>(<a href="T_CommandLine_Text_Example">Example</a>)))

## See Also


#### Reference
<a href="T_CommandLine_Text_HelpText">HelpText Class</a><br /><a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />