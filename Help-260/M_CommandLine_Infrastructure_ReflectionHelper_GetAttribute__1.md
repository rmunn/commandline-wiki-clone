# ReflectionHelper.GetAttribute(*TAttribute*) Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Infrastructure">CommandLine.Infrastructure</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static Maybe<TAttribute> GetAttribute<TAttribute>()
where TAttribute : Attribute

```

**VB**<br />
``` VB
Public Shared Function GetAttribute(Of TAttribute As Attribute) As Maybe(Of TAttribute)
```

**C++**<br />
``` C++
public:
generic<typename TAttribute>
where TAttribute : Attribute
static Maybe<TAttribute>^ GetAttribute()
```

**F#**<br />
``` F#
static member GetAttribute : unit -> Maybe<'TAttribute>  when 'TAttribute : Attribute

```


#### Type Parameters
&nbsp;<dl><dt>TAttribute</dt><dd /></dl>

#### Return Value
Type: <a href="T_CSharpx_Maybe_1">Maybe</a>(*TAttribute*)

## See Also


#### Reference
<a href="T_CommandLine_Infrastructure_ReflectionHelper">ReflectionHelper Class</a><br /><a href="N_CommandLine_Infrastructure">CommandLine.Infrastructure Namespace</a><br />