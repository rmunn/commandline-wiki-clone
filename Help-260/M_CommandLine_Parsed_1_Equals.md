# Parsed(*T*).Equals Method (Parsed(*T*))
 

Returns a value that indicates whether the current instance and a specified <a href="T_CommandLine_Parsed_1">Parsed(T)</a> have the same value.

**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public bool Equals(
	Parsed<T> other
)
```

**VB**<br />
``` VB
Public Function Equals ( 
	other As Parsed(Of T)
) As Boolean
```

**C++**<br />
``` C++
public:
virtual bool Equals(
	Parsed<T>^ other
) sealed
```

**F#**<br />
``` F#
abstract Equals : 
        other : Parsed<'T> -> bool 
override Equals : 
        other : Parsed<'T> -> bool 
```


#### Parameters
&nbsp;<dl><dt>other</dt><dd>Type: <a href="T_CommandLine_Parsed_1">CommandLine.Parsed</a>(<a href="T_CommandLine_Parsed_1">*T*</a>)<br />The <a href="T_CommandLine_Parsed_1">Parsed(T)</a> instance to compare.</dd></dl>

#### Return Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">Boolean</a><br />

#### Field Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">Boolean</a><br />true if this instance of <a href="T_CommandLine_Parsed_1">Parsed(T)</a> and *other* have the same value; otherwise, 

#### Field Value
Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">Boolean</a><br />false.

#### Implements
<a href="https://docs.microsoft.com/dotnet/api/system.iequatable-1.equals#System_IEquatable_1_Equals__0_" target="_blank">IEquatable(T).Equals(T)</a><br />

## See Also


#### Reference
<a href="T_CommandLine_Parsed_1">Parsed(T) Class</a><br /><a href="Overload_CommandLine_Parsed_1_Equals">Equals Overload</a><br /><a href="N_CommandLine">CommandLine Namespace</a><br />