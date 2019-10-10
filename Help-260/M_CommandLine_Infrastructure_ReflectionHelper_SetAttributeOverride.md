# ReflectionHelper.SetAttributeOverride Method 
 

Assembly attribute overrides for testing.

**Namespace:**&nbsp;<a href="N_CommandLine_Infrastructure">CommandLine.Infrastructure</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static void SetAttributeOverride(
	IEnumerable<Attribute> overrides
)
```

**VB**<br />
``` VB
Public Shared Sub SetAttributeOverride ( 
	overrides As IEnumerable(Of Attribute)
)
```

**C++**<br />
``` C++
public:
static void SetAttributeOverride(
	IEnumerable<Attribute^>^ overrides
)
```

**F#**<br />
``` F#
static member SetAttributeOverride : 
        overrides : IEnumerable<Attribute> -> unit 

```


#### Parameters
&nbsp;<dl><dt>overrides</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.ienumerable-1" target="_blank">System.Collections.Generic.IEnumerable</a>(<a href="https://docs.microsoft.com/dotnet/api/system.attribute" target="_blank">Attribute</a>)<br />Attributes that replace the existing assembly attributes or null, to clear any testing attributes.</dd></dl>

## Remarks
The implementation will fail if two or more attributes of the same type are included in *overrides*.

## See Also


#### Reference
<a href="T_CommandLine_Infrastructure_ReflectionHelper">ReflectionHelper Class</a><br /><a href="N_CommandLine_Infrastructure">CommandLine.Infrastructure Namespace</a><br />