# InstanceBuilder.BuildMutable(*T*) Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static T BuildMutable<T>(
	Maybe<Func<T>> factory,
	IEnumerable<SpecificationProperty> specPropsWithValue,
	List<Error> setPropertyErrors
)

```

**VB**<br />
``` VB
Private Shared Function BuildMutable(Of T) ( 
	factory As Maybe(Of Func(Of T)),
	specPropsWithValue As IEnumerable(Of SpecificationProperty),
	setPropertyErrors As List(Of Error)
) As T
```

**C++**<br />
``` C++
private:
generic<typename T>
static T BuildMutable(
	Maybe<Func<T>^>^ factory, 
	IEnumerable<SpecificationProperty^>^ specPropsWithValue, 
	List<Error^>^ setPropertyErrors
)
```

**F#**<br />
``` F#
private static member BuildMutable : 
        factory : Maybe<Func<'T>> * 
        specPropsWithValue : IEnumerable<SpecificationProperty> * 
        setPropertyErrors : List<Error> -> 'T 

```


#### Parameters
&nbsp;<dl><dt>factory</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.func-1" target="_blank">Func</a>(*T*))<br /></dd><dt>specPropsWithValue</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="T_CommandLine_Core_SpecificationProperty">SpecificationProperty</a>)<br /></dd><dt>setPropertyErrors</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.list-1" target="_blank">System.Collections.Generic.List</a>(<a href="T_CommandLine_Error">Error</a>)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: *T*

## See Also


#### Reference
<a href="T_CommandLine_Core_InstanceBuilder">InstanceBuilder Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />