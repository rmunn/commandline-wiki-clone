# SentenceBuilder Class
 

Exposes standard delegates to provide a mean to customize part of help screen generation. This type is consumed by <a href="T_CommandLine_Text_HelpText">HelpText</a>.


## Inheritance Hierarchy
<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br />&nbsp;&nbsp;CommandLine.Text.SentenceBuilder<br />&nbsp;&nbsp;&nbsp;&nbsp;<a href="T_CommandLine_Text_SentenceBuilder_DefaultSentenceBuilder">CommandLine.Text.SentenceBuilder.DefaultSentenceBuilder</a><br />
**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public abstract class SentenceBuilder
```

**VB**<br />
``` VB
Public MustInherit Class SentenceBuilder
```

**C++**<br />
``` C++
public ref class SentenceBuilder abstract
```

**F#**<br />
``` F#
[<AbstractClassAttribute>]
type SentenceBuilder =  class end
```

The SentenceBuilder type exposes the following members.


## Constructors
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Private method](media/privmethod.gif "Private method")![Static member](media/static.gif "Static member")</td><td><a href="M_CommandLine_Text_SentenceBuilder__cctor">SentenceBuilder</a></td><td /></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="M_CommandLine_Text_SentenceBuilder__ctor">SentenceBuilder</a></td><td>
Initializes a new instance of the SentenceBuilder class</td></tr></table>&nbsp;
<a href="#sentencebuilder-class">Back to Top</a>

## Properties
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_SentenceBuilder_ErrorsHeadingText">ErrorsHeadingText</a></td><td>
Gets a delegate that returns that errors block heading text.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")![Static member](media/static.gif "Static member")</td><td><a href="P_CommandLine_Text_SentenceBuilder_Factory">Factory</a></td><td>
Factory to allow custom SentenceBuilder injection</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_SentenceBuilder_FormatError">FormatError</a></td><td>
Gets a delegate that handles singular error formatting. The delegates must accept an <a href="T_CommandLine_Error">Error</a> and returns a string.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_SentenceBuilder_FormatMutuallyExclusiveSetErrors">FormatMutuallyExclusiveSetErrors</a></td><td>
Gets a delegate that handles mutually exclusive set errors formatting. The delegates must accept a sequence of <a href="T_CommandLine_MutuallyExclusiveSetError">MutuallyExclusiveSetError</a> and returns a string.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_SentenceBuilder_HelpCommandText">HelpCommandText</a></td><td>
Get a delegate that returns the help text of help command. The delegates must accept a boolean that is equal 

#### Field Value
Type: <br />true for options; otherwise 

#### Field Value
Type: <br />false for verbs.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_SentenceBuilder_RequiredWord">RequiredWord</a></td><td>
Gets a delegate that returns the word 'required'.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_SentenceBuilder_UsageHeadingText">UsageHeadingText</a></td><td>
Gets a delegate that returns usage text block heading text.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_SentenceBuilder_VersionCommandText">VersionCommandText</a></td><td>
Get a delegate that returns the help text of vesion command. The delegates must accept a boolean that is equal 

#### Field Value
Type: <br />true for options; otherwise 

#### Field Value
Type: <br />false for verbs.</td></tr></table>&nbsp;
<a href="#sentencebuilder-class">Back to Top</a>

## Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CommandLine_Text_SentenceBuilder_Create">Create</a></td><td>
Create instance of SentenceBuilder,</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.equals#System_Object_Equals_System_Object_" target="_blank">Equals</a></td><td>
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
<a href="#sentencebuilder-class">Back to Top</a>

## Extension Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_IsEmpty">IsEmpty</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_NormalizeValue">NormalizeValue</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr></table>&nbsp;
<a href="#sentencebuilder-class">Back to Top</a>

## See Also


#### Reference
<a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />