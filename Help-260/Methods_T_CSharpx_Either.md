# Either Methods
 

The <a href="T_CSharpx_Either">Either</a> type exposes the following members.


## Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_Either_Bimap__4">Bimap(TLeft, TRight, TLeft1, TRight1)</a></td><td>
Maps both parts of a Either type. Applies the first function if Either is Left. Otherwise applies the second function.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_Either_Bind__3">Bind(TLeft, TRight, TResult)</a></td><td>
Monadic bind.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_Either_Cast__1">Cast(TRight)</a></td><td>
Attempts to cast an object. Stores the cast value in 1Of2 if successful, otherwise stores the exception in 2Of2</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_Either_Fail__1">Fail(TRight)</a></td><td>
Fail with a message. Not part of mathematical definition of a monad.</td></tr><tr><td>![Private method](media/privmethod.gif "Private method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_Either_GetLeft__2">GetLeft(TLeft, TRight)</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_Either_GetLeftOrDefault__2">GetLeftOrDefault(TLeft, TRight)</a></td><td>
Returns a Either Left or a defualt value.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_Either_GetOrFail__2">GetOrFail(TLeft, TRight)</a></td><td>
Returns a Either Right or fail with an exception.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_Either_GetRightOrDefault__2">GetRightOrDefault(TLeft, TRight)</a></td><td>
Returns a Either Right or a defualt value.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_Either_Left__2">Left(TLeft, TRight)</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_Either_Map__3">Map(TLeft, TRight, TResult)</a></td><td>
Transforms a Either's right value by using a specified mapping function.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_Either_OfMaybe__2">OfMaybe(TLeft, TRight)</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_Either_Return__1">Return(TRight)</a></td><td>
Inject a value into the Either type, returning Right case.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_Either_Right__2">Right(TLeft, TRight)</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_Either_Select__3">Select(TLeft, TRight, TResult)</a></td><td>
Map operation compatible with Linq.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_Either_SelectMany__3">SelectMany(TLeft, TRight, TResult)</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CSharpx_Either_Try__1">Try(TRight)</a></td><td>
Wraps a function, encapsulates any exception thrown within to a Either.</td></tr></table>&nbsp;
<a href="#either-methods">Back to Top</a>

## See Also


#### Reference
<a href="T_CSharpx_Either">Either Class</a><br /><a href="N_CSharpx">CSharpx Namespace</a><br />