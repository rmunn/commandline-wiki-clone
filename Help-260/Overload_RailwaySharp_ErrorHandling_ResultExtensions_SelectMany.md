# ResultExtensions.SelectMany Method 
 


## Overload List
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_ResultExtensions_SelectMany__3">SelectMany(TSuccess, TMessage, TResult)(Result(TSuccess, TMessage), Func(TSuccess, Result(TResult, TMessage)))</a></td><td>
If the result is a Success it executes the given Func on the value. Otherwise the exisiting failure is propagated.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_RailwaySharp_ErrorHandling_ResultExtensions_SelectMany__4">SelectMany(TSuccess, TMessage, TValue, TResult)(Result(TSuccess, TMessage), Func(TSuccess, Result(TValue, TMessage)), Func(TSuccess, TValue, TResult))</a></td><td>
If the result is a Success it executes the given Func on the value. If the result of the Func is a Success it maps it using the given Func. Otherwise the exisiting failure is propagated.</td></tr></table>&nbsp;
<a href="#resultextensions.selectmany-method">Back to Top</a>

## See Also


#### Reference
<a href="T_RailwaySharp_ErrorHandling_ResultExtensions">ResultExtensions Class</a><br /><a href="N_RailwaySharp_ErrorHandling">RailwaySharp.ErrorHandling Namespace</a><br />