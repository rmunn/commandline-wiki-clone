# Maybe(*T*) Class
 

The Maybe type models an optional value. A value of type Maybe a either contains a value of type a (represented as Just a), or it is empty (represented as Nothing).


## Inheritance Hierarchy
<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br />&nbsp;&nbsp;CSharpx.Maybe(T)<br />&nbsp;&nbsp;&nbsp;&nbsp;<a href="T_CSharpx_Just_1">CSharpx.Just(T)</a><br />&nbsp;&nbsp;&nbsp;&nbsp;<a href="T_CSharpx_Nothing_1">CSharpx.Nothing(T)</a><br />
**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
internal abstract class Maybe<T>

```

**VB**<br />
``` VB
Friend MustInherit Class Maybe(Of T)
```

**C++**<br />
``` C++
generic<typename T>
internal ref class Maybe abstract
```

**F#**<br />
``` F#
[<AbstractClassAttribute>]
type Maybe<'T> =  class end
```


#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>&nbsp;
The Maybe(T) type exposes the following members.


## Constructors
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="M_CSharpx_Maybe_1__ctor">Maybe(T)</a></td><td>
Initializes a new instance of the Maybe(T) class</td></tr></table>&nbsp;
<a href="#maybe(*t*)-class">Back to Top</a>

## Properties
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CSharpx_Maybe_1_Tag">Tag</a></td><td>
Type discriminator.</td></tr></table>&nbsp;
<a href="#maybe(*t*)-class">Back to Top</a>

## Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.equals#System_Object_Equals_System_Object_" target="_blank">Equals</a></td><td>
Determines whether the specified object is equal to the current object.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.finalize#System_Object_Finalize" target="_blank">Finalize</a></td><td>
Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.gethashcode#System_Object_GetHashCode" target="_blank">GetHashCode</a></td><td>
Serves as the default hash function.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.gettype#System_Object_GetType" target="_blank">GetType</a></td><td>
Gets the <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a> of the current instance.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CSharpx_Maybe_1_MatchJust">MatchJust</a></td><td>
Matches a value returning `true` and value itself via output parameter.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CSharpx_Maybe_1_MatchNothing">MatchNothing</a></td><td>
Matches an empty value returning `true`.</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.memberwiseclone#System_Object_MemberwiseClone" target="_blank">MemberwiseClone</a></td><td>
Creates a shallow copy of the current <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.tostring#System_Object_ToString" target="_blank">ToString</a></td><td>
Returns a string that represents the current object.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr></table>&nbsp;
<a href="#maybe(*t*)-class">Back to Top</a>

## Extension Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_MaybeExtensions_Bind__2">Bind(T1, T2)</a></td><td>
Invokes a function on this maybe value that itself yields a maybe.
 (Defined by <a href="T_CSharpx_MaybeExtensions">MaybeExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_MaybeExtensions_Do__1">Do(T)</a></td><td>
If contans a value executes an <a href="https://docs.microsoft.com/dotnet/api/system.action-1" target="_blank">Action(T)</a> delegate over it.
 (Defined by <a href="T_CSharpx_MaybeExtensions">MaybeExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_MaybeExtensions_FromJust__1">FromJust(T)</a></td><td>
Extracts the element out of a <a href="T_CSharpx_Just_1">Just(T)</a> and returns a default value if its argument is <a href="T_CSharpx_Nothing_1">Nothing(T)</a>.
 (Defined by <a href="T_CSharpx_MaybeExtensions">MaybeExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_MaybeExtensions_FromJustOrFail__1">FromJustOrFail(T)</a></td><td>
Extracts the element out of a <a href="T_CSharpx_Just_1">Just(T)</a> and throws an error if its argument is <a href="T_CSharpx_Nothing_1">Nothing(T)</a>.
 (Defined by <a href="T_CSharpx_MaybeExtensions">MaybeExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_MaybeExtensions_GetValueOrDefault__1">GetValueOrDefault(T)</a></td><td>
If contains a values returns it, otherwise returns *noneValue*.
 (Defined by <a href="T_CSharpx_MaybeExtensions">MaybeExtensions</a>.)</td></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_IsEmpty">IsEmpty</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_MaybeExtensions_IsJust__1">IsJust(T)</a></td><td>
Returns `true` iffits argument is of the form <a href="T_CSharpx_Just_1">Just(T)</a>.
 (Defined by <a href="T_CSharpx_MaybeExtensions">MaybeExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_MaybeExtensions_IsNothing__1">IsNothing(T)</a></td><td>
Returns `true` iffits argument is of the form <a href="T_CSharpx_Nothing_1">Nothing(T)</a>.
 (Defined by <a href="T_CSharpx_MaybeExtensions">MaybeExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_MaybeExtensions_Map__2">Map(T1, T2)</a></td><td>
Transforms this maybe value by using a specified mapping function.
 (Defined by <a href="T_CSharpx_MaybeExtensions">MaybeExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_MaybeExtensions_MapValueOrDefault__2">MapValueOrDefault(T1, T2)</a></td><td>
If contains a values executes a mapping function over it, otherwise returns *noneValue*.
 (Defined by <a href="T_CSharpx_MaybeExtensions">MaybeExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_MaybeExtensions_Match__1">Match(T)</a></td><td>
Provides pattern matching using <a href="https://docs.microsoft.com/dotnet/api/system.action" target="_blank">Action</a> delegates.
 (Defined by <a href="T_CSharpx_MaybeExtensions">MaybeExtensions</a>.)</td></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_NormalizeValue">NormalizeValue</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_MaybeExtensions_Select__2">Select(TSource, TResult)</a></td><td>
Map operation compatible with Linq.
 (Defined by <a href="T_CSharpx_MaybeExtensions">MaybeExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_MaybeExtensions_SelectMany__3">SelectMany(TSource, TValue, TResult)</a></td><td>
Bind operation compatible with Linq.
 (Defined by <a href="T_CSharpx_MaybeExtensions">MaybeExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_MaybeExtensions_ToEnumerable__1">ToEnumerable(T)</a></td><td>
Returns an empty list when given <a href="T_CSharpx_Nothing_1">Nothing(T)</a> or a singleton list when given a <a href="T_CSharpx_Just_1">Just(T)</a>.
 (Defined by <a href="T_CSharpx_MaybeExtensions">MaybeExtensions</a>.)</td></tr></table>&nbsp;
<a href="#maybe(*t*)-class">Back to Top</a>

## See Also


#### Reference
<a href="N_CSharpx">CSharpx Namespace</a><br />