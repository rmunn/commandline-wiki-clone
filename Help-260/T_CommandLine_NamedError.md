# NamedError Class
 

Base type of all erros with name information.


## Inheritance Hierarchy
<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br />&nbsp;&nbsp;<a href="T_CommandLine_Error">CommandLine.Error</a><br />&nbsp;&nbsp;&nbsp;&nbsp;CommandLine.NamedError<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#inheritance-hierarchy">More...</a>
**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public abstract class NamedError : Error, 
	IEquatable<NamedError>
```

**VB**<br />
``` VB
Public MustInherit Class NamedError
	Inherits Error
	Implements IEquatable(Of NamedError)
```

**C++**<br />
``` C++
public ref class NamedError abstract : public Error, 
	IEquatable<NamedError^>
```

**F#**<br />
``` F#
[<AbstractClassAttribute>]
type NamedError =  
    class
        inherit Error
        interface IEquatable<NamedError>
    end
```

The NamedError type exposes the following members.


## Constructors
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="M_CommandLine_NamedError__ctor">NamedError</a></td><td>
Initializes a new instance of the NamedError class.</td></tr></table>&nbsp;
<a href="#namederror-class">Back to Top</a>

## Properties
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_NamedError_NameInfo">NameInfo</a></td><td>
Name information relative to this error instance.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Error_StopsProcessing">StopsProcessing</a></td><td>
Tells if error stops parsing process. Filtered by <a href="M_CommandLine_ErrorExtensions_OnlyMeaningfulOnes">OnlyMeaningfulOnes(IEnumerable(Error))</a>.
 (Inherited from <a href="T_CommandLine_Error">Error</a>.)</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Error_Tag">Tag</a></td><td>
Error type discriminator, defined as <a href="T_CommandLine_ErrorType">ErrorType</a> enumeration.
 (Inherited from <a href="T_CommandLine_Error">Error</a>.)</td></tr></table>&nbsp;
<a href="#namederror-class">Back to Top</a>

## Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_NamedError_Equals_1">Equals(Object)</a></td><td>
Determines whether the specified <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a> is equal to the current <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.
 (Overrides <a href="M_CommandLine_Error_Equals_1">Error.Equals(Object)</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Error_Equals">Equals(Error)</a></td><td>
Returns a value that indicates whether the current instance and a specified <a href="T_CommandLine_Error">Error</a> have the same value.
 (Inherited from <a href="T_CommandLine_Error">Error</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_NamedError_Equals">Equals(NamedError)</a></td><td>
Returns a value that indicates whether the current instance and a specified NamedError have the same value.</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.finalize#System_Object_Finalize" target="_blank">Finalize</a></td><td>
Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_NamedError_GetHashCode">GetHashCode</a></td><td>
Serves as a hash function for a particular type.
 (Overrides <a href="M_CommandLine_Error_GetHashCode">Error.GetHashCode()</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.gettype#System_Object_GetType" target="_blank">GetType</a></td><td>
Gets the <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a> of the current instance.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.memberwiseclone#System_Object_MemberwiseClone" target="_blank">MemberwiseClone</a></td><td>
Creates a shallow copy of the current <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.tostring#System_Object_ToString" target="_blank">ToString</a></td><td>
Returns a string that represents the current object.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr></table>&nbsp;
<a href="#namederror-class">Back to Top</a>

## Extension Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_IsEmpty">IsEmpty</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_NormalizeValue">NormalizeValue</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr></table>&nbsp;
<a href="#namederror-class">Back to Top</a>

## See Also


#### Reference
<a href="N_CommandLine">CommandLine Namespace</a><br />

## Inheritance Hierarchy<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br />&nbsp;&nbsp;<a href="T_CommandLine_Error">CommandLine.Error</a><br />&nbsp;&nbsp;&nbsp;&nbsp;CommandLine.NamedError<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="T_CommandLine_BadFormatConversionError">CommandLine.BadFormatConversionError</a><br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="T_CommandLine_MissingRequiredOptionError">CommandLine.MissingRequiredOptionError</a><br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="T_CommandLine_MissingValueOptionError">CommandLine.MissingValueOptionError</a><br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="T_CommandLine_MutuallyExclusiveSetError">CommandLine.MutuallyExclusiveSetError</a><br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="T_CommandLine_RepeatedOptionError">CommandLine.RepeatedOptionError</a><br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="T_CommandLine_SequenceOutOfRangeError">CommandLine.SequenceOutOfRangeError</a><br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="T_CommandLine_SetValueExceptionError">CommandLine.SetValueExceptionError</a><br />