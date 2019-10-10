# EnumerableExtensions.MaterializedEnumerable(*T*) Class
 


## Inheritance Hierarchy
<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br />&nbsp;&nbsp;CSharpx.EnumerableExtensions.MaterializedEnumerable(T)<br />
**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
private class MaterializedEnumerable<T> : IEnumerable<T>, 
	IEnumerable

```

**VB**<br />
``` VB
Private Class MaterializedEnumerable(Of T)
	Implements IEnumerable(Of T), IEnumerable
```

**C++**<br />
``` C++
generic<typename T>
private ref class MaterializedEnumerable : IEnumerable<T>, 
	IEnumerable
```

**F#**<br />
``` F#
type MaterializedEnumerable<'T> =  
    class
        interface IEnumerable<'T>
        interface IEnumerable
    end
```


#### Type Parameters
&nbsp;<dl><dt>T</dt><dd /></dl>&nbsp;
The EnumerableExtensions.MaterializedEnumerable(T) type exposes the following members.


## Constructors
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CSharpx_EnumerableExtensions_MaterializedEnumerable_1__ctor">EnumerableExtensions.MaterializedEnumerable(T)</a></td><td>
Initializes a new instance of the EnumerableExtensions.MaterializedEnumerable(T) class</td></tr></table>&nbsp;
<a href="#enumerableextensions.materializedenumerable(*t*)-class">Back to Top</a>

## Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.equals#System_Object_Equals_System_Object_" target="_blank">Equals</a></td><td>
Determines whether the specified object is equal to the current object.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.finalize#System_Object_Finalize" target="_blank">Finalize</a></td><td>
Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CSharpx_EnumerableExtensions_MaterializedEnumerable_1_GetEnumerator">GetEnumerator</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.gethashcode#System_Object_GetHashCode" target="_blank">GetHashCode</a></td><td>
Serves as the default hash function.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.gettype#System_Object_GetType" target="_blank">GetType</a></td><td>
Gets the <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a> of the current instance.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.memberwiseclone#System_Object_MemberwiseClone" target="_blank">MemberwiseClone</a></td><td>
Creates a shallow copy of the current <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.tostring#System_Object_ToString" target="_blank">ToString</a></td><td>
Returns a string that represents the current object.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr></table>&nbsp;
<a href="#enumerableextensions.materializedenumerable(*t*)-class">Back to Top</a>

## Extension Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_EnumerableExtensions_Cartesian__3">Cartesian(T, TSecond, TResult)</a></td><td>
Returns the Cartesian product of two sequences by combining each element of the first set with each in the second and applying the user=define projection to the pair.
 (Defined by <a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_EnumerableExtensions_Concat__1">Concat(T)</a></td><td>
Returns a sequence consisting of the head elements and the given tail element.
 (Defined by <a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_Core_SpecificationPropertyRules_ContainsIfNotEmpty__1">ContainsIfNotEmpty(T)</a></td><td> (Defined by <a href="T_CommandLine_Core_SpecificationPropertyRules">SpecificationPropertyRules</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CommandLine_Infrastructure_EnumerableExtensions_Empty__1">Empty(T)</a></td><td> (Defined by <a href="T_CommandLine_Infrastructure_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_EnumerableExtensions_Exclude__1">Exclude(T)</a></td><td>
Excludes *count* elements from a sequence starting at a given index
 (Defined by <a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_EnumerableExtensions_Fold__2">Fold(T, TResult)(Func(T, TResult))</a></td><td>Overloaded.  
Returns the result of applying a function to a sequence of 1 element.
 (Defined by <a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_EnumerableExtensions_Fold__2_1">Fold(T, TResult)(Func(T, T, TResult))</a></td><td>Overloaded.  
Returns the result of applying a function to a sequence of 2 elements.
 (Defined by <a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_EnumerableExtensions_Fold__2_2">Fold(T, TResult)(Func(T, T, T, TResult))</a></td><td>Overloaded.  
Returns the result of applying a function to a sequence of 3 elements.
 (Defined by <a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_EnumerableExtensions_Fold__2_3">Fold(T, TResult)(Func(T, T, T, T, TResult))</a></td><td>Overloaded.  
Returns the result of applying a function to a sequence of 4 elements.
 (Defined by <a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_EnumerableExtensions_ForEach__1">ForEach(T)</a></td><td>
Immediately executes the given action on each element in the source sequence.
 (Defined by <a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CommandLine_Infrastructure_EnumerableExtensions_Group__1">Group(T)</a></td><td>
Breaks a collection into groups of a specified size.
 (Defined by <a href="T_CommandLine_Infrastructure_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_EnumerableExtensions_Index__1">Index(T)()</a></td><td>Overloaded.  
Returns a sequence of <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.keyvaluepair-2" target="_blank">KeyValuePair(TKey, TValue)</a> where the key is the zero-based index of the value in the source sequence.
 (Defined by <a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_EnumerableExtensions_Index__1_1">Index(T)(Int32)</a></td><td>Overloaded.  
Returns a sequence of <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.keyvaluepair-2" target="_blank">KeyValuePair(TKey, TValue)</a> where the key is the index of the value in the source sequence. An additional parameter specifies the starting index.
 (Defined by <a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CommandLine_Infrastructure_EnumerableExtensions_IndexOf__1">IndexOf(T)</a></td><td> (Defined by <a href="T_CommandLine_Infrastructure_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_IsEmpty">IsEmpty</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_EnumerableExtensions_Materialize__1">Materialize(T)</a></td><td>
Creates an immutable copy of a sequence.
 (Defined by <a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_EnumerableExtensions_Memorize__1">Memorize(T)</a></td><td>
Captures current state of a sequence.
 (Defined by <a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_NormalizeValue">NormalizeValue</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_EnumerableExtensions_Pairwise__2">Pairwise(T, TResult)</a></td><td>
Returns a sequence resulting from applying a function to each element in the source sequence and its predecessor, with the exception of the first element which is only returned as the predecessor of the second element.
 (Defined by <a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CSharpx_EnumerableExtensions_PairwiseImpl__2">PairwiseImpl(T, TResult)</a></td><td> (Defined by <a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_EnumerableExtensions_Prepend__1">Prepend(T)</a></td><td>
Prepends a single value to a sequence.
 (Defined by <a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_EnumerableExtensions_Tail__1">Tail(T)</a></td><td>
Return everything except first element and throws exception if empty.
 (Defined by <a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_EnumerableExtensions_TailNoFail__1">TailNoFail(T)</a></td><td>
Return everything except first element without throwing exception if empty.
 (Defined by <a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_EnumerableExtensions_ToDelimitedString__1">ToDelimitedString(T)()</a></td><td>Overloaded.  
Creates a delimited string from a sequence of values. The delimiter used depends on the current culture of the executing thread.
 (Defined by <a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_EnumerableExtensions_ToDelimitedString__1_1">ToDelimitedString(T)(String)</a></td><td>Overloaded.  
Creates a delimited string from a sequence of values and a given delimiter.
 (Defined by <a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_EnumerableExtensions_ToMaybe__1">ToMaybe(T)</a></td><td>
Turns an empty sequence to Nothing, otherwise Just(sequence).
 (Defined by <a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CSharpx_EnumerableExtensions_TryHead__1">TryHead(T)</a></td><td>
Safe function that returns Just(first element) or None.
 (Defined by <a href="T_CSharpx_EnumerableExtensions">EnumerableExtensions</a>.)</td></tr></table>&nbsp;
<a href="#enumerableextensions.materializedenumerable(*t*)-class">Back to Top</a>

## Explicit Interface Implementations
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Explicit interface implementation](media/pubinterface.gif "Explicit interface implementation")![Private method](media/privmethod.gif "Private method")</td><td><a href="M_CSharpx_EnumerableExtensions_MaterializedEnumerable_1_System_Collections_IEnumerable_GetEnumerator">IEnumerable.GetEnumerator</a></td><td /></tr></table>&nbsp;
<a href="#enumerableextensions.materializedenumerable(*t*)-class">Back to Top</a>

## See Also


#### Reference
<a href="N_CSharpx">CSharpx Namespace</a><br />