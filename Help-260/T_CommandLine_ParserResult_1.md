# ParserResult(*T*) Class
 

Models a parser result. When inherited by <a href="T_CommandLine_Parsed_1">Parsed(T)</a>, it contains an instance of type *T* with parsed values. When inherited by <a href="T_CommandLine_NotParsed_1">NotParsed(T)</a>, it contains a sequence of <a href="T_CommandLine_Error">Error</a>.


## Inheritance Hierarchy
<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br />&nbsp;&nbsp;CommandLine.ParserResult(T)<br />&nbsp;&nbsp;&nbsp;&nbsp;<a href="T_CommandLine_NotParsed_1">CommandLine.NotParsed(T)</a><br />&nbsp;&nbsp;&nbsp;&nbsp;<a href="T_CommandLine_Parsed_1">CommandLine.Parsed(T)</a><br />
**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public abstract class ParserResult<T>

```

**VB**<br />
``` VB
Public MustInherit Class ParserResult(Of T)
```

**C++**<br />
``` C++
generic<typename T>
public ref class ParserResult abstract
```

**F#**<br />
``` F#
[<AbstractClassAttribute>]
type ParserResult<'T> =  class end
```


#### Type Parameters
&nbsp;<dl><dt>T</dt><dd>The type with attributes that define the syntax of parsing rules.</dd></dl>&nbsp;
The ParserResult(T) type exposes the following members.


## Constructors
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="M_CommandLine_ParserResult_1__ctor">ParserResult(T)</a></td><td>
Initializes a new instance of the ParserResult(T) class</td></tr></table>&nbsp;
<a href="#parserresult(*t*)-class">Back to Top</a>

## Properties
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_ParserResult_1_Tag">Tag</a></td><td>
Parser result type discriminator, defined as <a href="T_CommandLine_ParserResultType">ParserResultType</a> enumeration.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_ParserResult_1_TypeInfo">TypeInfo</a></td><td /></tr></table>&nbsp;
<a href="#parserresult(*t*)-class">Back to Top</a>

## Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.equals#System_Object_Equals_System_Object_" target="_blank">Equals</a></td><td>
Determines whether the specified object is equal to the current object.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.finalize#System_Object_Finalize" target="_blank">Finalize</a></td><td>
Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.gethashcode#System_Object_GetHashCode" target="_blank">GetHashCode</a></td><td>
Serves as the default hash function.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.gettype#System_Object_GetType" target="_blank">GetType</a></td><td>
Gets the <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a> of the current instance.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.memberwiseclone#System_Object_MemberwiseClone" target="_blank">MemberwiseClone</a></td><td>
Creates a shallow copy of the current <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.tostring#System_Object_ToString" target="_blank">ToString</a></td><td>
Returns a string that represents the current object.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr></table>&nbsp;
<a href="#parserresult(*t*)-class">Back to Top</a>

## Extension Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_IsEmpty">IsEmpty</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CommandLine_ParserResultExtensions_MapResult__2_1">MapResult(TSource, TResult)</a></td><td>
Provides a way to transform result data into another value.
 (Defined by <a href="T_CommandLine_ParserResultExtensions">ParserResultExtensions</a>.)</td></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_NormalizeValue">NormalizeValue</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CommandLine_ParserResultExtensions_WithNotParsed__1">WithNotParsed(T)</a></td><td>
Executes *action* if ParserResult(T) lacks parsed values and contains errors.
 (Defined by <a href="T_CommandLine_ParserResultExtensions">ParserResultExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CommandLine_ParserResultExtensions_WithParsed__1_1">WithParsed(T)</a></td><td>
Executes *action* if ParserResult(T) contains parsed values.
 (Defined by <a href="T_CommandLine_ParserResultExtensions">ParserResultExtensions</a>.)</td></tr></table>&nbsp;
<a href="#parserresult(*t*)-class">Back to Top</a>

## See Also


#### Reference
<a href="N_CommandLine">CommandLine Namespace</a><br />