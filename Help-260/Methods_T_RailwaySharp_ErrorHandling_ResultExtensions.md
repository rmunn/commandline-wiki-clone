# ResultExtensions Methods
 

The <a href="T_RailwaySharp_ErrorHandling_ResultExtensions">ResultExtensions</a> type exposes the following members.


## Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_ResultExtensions_Collect__2">Collect(TSuccess, TMessage)</a></td><td>
Collects a sequence of Results and accumulates their values. If the sequence contains an error the error will be propagated.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_ResultExtensions_Either__3">Either(TSuccess, TMessage, TResult)</a></td><td>
Allows pattern matching on Results.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_ResultExtensions_FailedWith__2">FailedWith(TSuccess, TMessage)</a></td><td>
Returns the error messages or fails if the result was a success.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_ResultExtensions_Flatten__2">Flatten(TSuccess, TMessage)</a></td><td>
Collects a sequence of Results and accumulates their values. If the sequence contains an error the error will be propagated.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_ResultExtensions_Map__3">Map(TSuccess, TMessage, TResult)</a></td><td>
Lifts a Func into a Result and applies it on the given result.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_ResultExtensions_Match__2">Match(TSuccess, TMessage)</a></td><td>
Allows pattern matching on Results.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_ResultExtensions_Select__3">Select(TSuccess, TMessage, TResult)</a></td><td>
Lifts a Func into a Result and applies it on the given result.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_ResultExtensions_SelectMany__3">SelectMany(TSuccess, TMessage, TResult)(Result(TSuccess, TMessage), Func(TSuccess, Result(TResult, TMessage)))</a></td><td>
If the result is a Success it executes the given Func on the value. Otherwise the exisiting failure is propagated.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_ResultExtensions_SelectMany__4">SelectMany(TSuccess, TMessage, TValue, TResult)(Result(TSuccess, TMessage), Func(TSuccess, Result(TValue, TMessage)), Func(TSuccess, TValue, TResult))</a></td><td>
If the result is a Success it executes the given Func on the value. If the result of the Func is a Success it maps it using the given Func. Otherwise the exisiting failure is propagated.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_ResultExtensions_SucceededWith__2">SucceededWith(TSuccess, TMessage)</a></td><td>
Returns the result or fails if the result was an error.</td></tr></table>&nbsp;
<a href="#resultextensions-methods">Back to Top</a>

## See Also


#### Reference
<a href="T_RailwaySharp_ErrorHandling_ResultExtensions">ResultExtensions Class</a><br /><a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling Namespace</a><br />