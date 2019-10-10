# InstanceBuilder.BuildImmutable(*T*) Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Core">CommandLine.Core</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private static T BuildImmutable<T>(
	Type typeInfo,
	Maybe<Func<T>> factory,
	IEnumerable<SpecificationProperty> specProps,
	IEnumerable<SpecificationProperty> specPropsWithValue,
	List<Error> setPropertyErrors
)

```

**VB**<br />
``` VB
Private Shared Function BuildImmutable(Of T) ( 
	typeInfo As Type,
	factory As Maybe(Of Func(Of T)),
	specProps As IEnumerable(Of SpecificationProperty),
	specPropsWithValue As IEnumerable(Of SpecificationProperty),
	setPropertyErrors As List(Of Error)
) As T
```

**C++**<br />
``` C++
private:
generic<typename T>
static T BuildImmutable(
	Type^ typeInfo, 
	Maybe<Func<T>^>^ factory, 
	IEnumerable<SpecificationProperty^>^ specProps, 
	IEnumerable<SpecificationProperty^>^ specPropsWithValue, 
	List<Error^>^ setPropertyErrors
)
```

**F#**<br />
``` F#
private static member BuildImmutable : 
        typeInfo : Type * 
        factory : Maybe<Func<'T>> * 
        specProps : IEnumerable<SpecificationProperty> * 
        specPropsWithValue : IEnumerable<SpecificationProperty> * 
        setPropertyErrors : List<Error> -> 'T 

```


#### Parameters
&nbsp;<dl><dt>typeInfo</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">System.Type</a><br /></dd><dt>factory</dt><dd>Type: <a href="T_CSharpx_Maybe_1">CSharpx.Maybe</a>(<a href="https://docs.microsoft.com/dotnet/api/system.func-1" target="_blank">Func</a>(*T*))<br /></dd><dt>specProps</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="T_CommandLine_Core_SpecificationProperty">SpecificationProperty</a>)<br /></dd><dt>specPropsWithValue</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="T_CommandLine_Core_SpecificationProperty">SpecificationProperty</a>)<br /></dd><dt>setPropertyErrors</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.list-1" target="_blank">System.Collections.Generic.List</a>(<a href="T_CommandLine_Error">Error</a>)<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

#### Return Value
Type: *T*

## See Also


#### Reference
<a href="T_CommandLine_Core_InstanceBuilder">InstanceBuilder Class</a><br /><a href="N_CommandLine_Core">CommandLine.Core Namespace</a><br />