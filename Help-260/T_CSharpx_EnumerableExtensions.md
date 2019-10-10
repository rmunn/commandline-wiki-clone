# EnumerableExtensions Class
 


## Inheritance Hierarchy
<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br />&nbsp;&nbsp;CSharpx.EnumerableExtensions<br />
**Namespace:**&nbsp;<a href="N_CSharpx">CSharpx</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
internal static class EnumerableExtensions
```

**VB**<br />
``` VB
<ExtensionAttribute>
Friend NotInheritable Class EnumerableExtensions
```

**C++**<br />
``` C++
[ExtensionAttribute]
internal ref class EnumerableExtensions abstract sealed
```

**F#**<br />
``` F#
[<AbstractClassAttribute>]
[<SealedAttribute>]
[<ExtensionAttribute>]
type EnumerableExtensions =  class end
```

The EnumerableExtensions type exposes the following members.


## Constructors
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Private method](media/privmethod.gif "Private method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions__cctor">EnumerableExtensions</a></td><td /></tr></table>&nbsp;
<a href="#enumerableextensions-class">Back to Top</a>

## Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Private method](media/privmethod.gif "Private method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_AssertCountImpl__1">AssertCountImpl(TSource)</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_Cartesian__3">Cartesian(TFirst, TSecond, TResult)</a></td><td>
Returns the Cartesian product of two sequences by combining each element of the first set with each in the second and applying the user=define projection to the pair.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_Concat__1">Concat(T)(IEnumerable(T), T)</a></td><td>
Returns a sequence consisting of the head elements and the given tail element.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_Concat__1_1">Concat(T)(T, IEnumerable(T))</a></td><td>
Returns a sequence consisting of the head element and the given tail elements.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_Exclude__1">Exclude(T)</a></td><td>
Excludes *count* elements from a sequence starting at a given index</td></tr><tr><td>![Private method](media/privmethod.gif "Private method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_ExcludeImpl__1">ExcludeImpl(T)</a></td><td /></tr><tr><td>![Private method](media/privmethod.gif "Private method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_ExpectingCountYieldingImpl__1">ExpectingCountYieldingImpl(TSource)</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_Fold__2">Fold(T, TResult)(IEnumerable(T), Func(T, TResult))</a></td><td>
Returns the result of applying a function to a sequence of 1 element.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_Fold__2_1">Fold(T, TResult)(IEnumerable(T), Func(T, T, TResult))</a></td><td>
Returns the result of applying a function to a sequence of 2 elements.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_Fold__2_2">Fold(T, TResult)(IEnumerable(T), Func(T, T, T, TResult))</a></td><td>
Returns the result of applying a function to a sequence of 3 elements.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_Fold__2_3">Fold(T, TResult)(IEnumerable(T), Func(T, T, T, T, TResult))</a></td><td>
Returns the result of applying a function to a sequence of 4 elements.</td></tr><tr><td>![Private method](media/privmethod.gif "Private method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_FoldImpl__2">FoldImpl(T, TResult)</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_ForEach__1">ForEach(T)</a></td><td>
Immediately executes the given action on each element in the source sequence.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_Index__1">Index(TSource)(IEnumerable(TSource))</a></td><td>
Returns a sequence of <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.keyvaluepair-2" target="_blank">KeyValuePair(TKey, TValue)</a> where the key is the zero-based index of the value in the source sequence.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_Index__1_1">Index(TSource)(IEnumerable(TSource), Int32)</a></td><td>
Returns a sequence of <a href="https://docs.microsoft.com/dotnet/api/system.collections.generic.keyvaluepair-2" target="_blank">KeyValuePair(TKey, TValue)</a> where the key is the index of the value in the source sequence. An additional parameter specifies the starting index.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_Materialize__1">Materialize(T)</a></td><td>
Creates an immutable copy of a sequence.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_Memorize__1">Memorize(T)</a></td><td>
Captures current state of a sequence.</td></tr><tr><td>![Private method](media/privmethod.gif "Private method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_OnFolderSourceSizeError">OnFolderSourceSizeError</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_Pairwise__2">Pairwise(TSource, TResult)</a></td><td>
Returns a sequence resulting from applying a function to each element in the source sequence and its predecessor, with the exception of the first element which is only returned as the predecessor of the second element.</td></tr><tr><td>![Private method](media/privmethod.gif "Private method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_PairwiseImpl__2">PairwiseImpl(TSource, TResult)</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_Prepend__1">Prepend(TSource)</a></td><td>
Prepends a single value to a sequence.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_Tail__1">Tail(T)</a></td><td>
Return everything except first element and throws exception if empty.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_TailNoFail__1">TailNoFail(T)</a></td><td>
Return everything except first element without throwing exception if empty.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_ToDelimitedString__1">ToDelimitedString(TSource)(IEnumerable(TSource))</a></td><td>
Creates a delimited string from a sequence of values. The delimiter used depends on the current culture of the executing thread.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_ToDelimitedString__1_1">ToDelimitedString(TSource)(IEnumerable(TSource), String)</a></td><td>
Creates a delimited string from a sequence of values and a given delimiter.</td></tr><tr><td>![Private method](media/privmethod.gif "Private method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_ToDelimitedStringImpl__1">ToDelimitedStringImpl(T)</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_ToMaybe__1">ToMaybe(T)</a></td><td>
Turns an empty sequence to Nothing, otherwise Just(sequence).</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_EnumerableExtensions_TryHead__1">TryHead(T)</a></td><td>
Safe function that returns Just(first element) or None.</td></tr></table>&nbsp;
<a href="#enumerableextensions-class">Back to Top</a>

## See Also


#### Reference
<a href="N_CSharpx">CSharpx Namespace</a><br />