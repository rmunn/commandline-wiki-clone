# PopsicleSetter.Set(*T*) Method 
 

**Namespace:**&nbsp;<a href="N_CommandLine_Infrastructure">CommandLine.Infrastructure</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public static void Set<T>(
	bool consumed,
	ref T field,
	T value
)

```

**VB**<br />
``` VB
Public Shared Sub Set(Of T) ( 
	consumed As Boolean,
	ByRef field As T,
	value As T
)
```

**C++**<br />
``` C++
public:
generic<typename T>
static void Set(
	bool consumed, 
	T% field, 
	T value
)
```

**F#**<br />
``` F#
static member Set : 
        consumed : bool * 
        field : 'T byref * 
        value : 'T -> unit 

```


#### Parameters
&nbsp;<dl><dt>consumed</dt><dd>Type: <a href="https://docs.microsoft.com/dotnet/api/system.boolean" target="_blank">System.Boolean</a><br /></dd><dt>field</dt><dd>Type: *T*<br /></dd><dt>value</dt><dd>Type: *T*<br /></dd></dl>

#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>

## See Also


#### Reference
<a href="T_CommandLine_Infrastructure_PopsicleSetter">PopsicleSetter Class</a><br /><a href="N_CommandLine_Infrastructure">CommandLine.Infrastructure Namespace</a><br />