# MultilineTextAttribute Class
 

Provides base properties for creating an attribute, used to define multiple lines of text.


## Inheritance Hierarchy
<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br />&nbsp;&nbsp;<a href="https://docs.microsoft.com/dotnet/api/system.attribute" target="_blank">System.Attribute</a><br />&nbsp;&nbsp;&nbsp;&nbsp;CommandLine.Text.MultilineTextAttribute<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="T_CommandLine_Text_AssemblyLicenseAttribute">CommandLine.Text.AssemblyLicenseAttribute</a><br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="T_CommandLine_Text_AssemblyUsageAttribute">CommandLine.Text.AssemblyUsageAttribute</a><br />
**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public abstract class MultilineTextAttribute : Attribute
```

**VB**<br />
``` VB
Public MustInherit Class MultilineTextAttribute
	Inherits Attribute
```

**C++**<br />
``` C++
public ref class MultilineTextAttribute abstract : public Attribute
```

**F#**<br />
``` F#
[<AbstractClassAttribute>]
type MultilineTextAttribute =  
    class
        inherit Attribute
    end
```

The MultilineTextAttribute type exposes the following members.


## Constructors
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="M_CommandLine_Text_MultilineTextAttribute__ctor">MultilineTextAttribute(String)</a></td><td>
Initializes a new instance of the MultilineTextAttribute class. Used in derived type using one line of text.</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="M_CommandLine_Text_MultilineTextAttribute__ctor_1">MultilineTextAttribute(String, String)</a></td><td>
Initializes a new instance of the MultilineTextAttribute class. Used in type using two lines of text.</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="M_CommandLine_Text_MultilineTextAttribute__ctor_2">MultilineTextAttribute(String, String, String)</a></td><td>
Initializes a new instance of the MultilineTextAttribute class. Used in type using three lines of text.</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="M_CommandLine_Text_MultilineTextAttribute__ctor_3">MultilineTextAttribute(String, String, String, String)</a></td><td>
Initializes a new instance of the MultilineTextAttribute class. Used in type using four lines of text.</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="M_CommandLine_Text_MultilineTextAttribute__ctor_4">MultilineTextAttribute(String, String, String, String, String)</a></td><td>
Initializes a new instance of the MultilineTextAttribute class. Used in type using five lines of text.</td></tr></table>&nbsp;
<a href="#multilinetextattribute-class">Back to Top</a>

## Properties
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_MultilineTextAttribute_Line1">Line1</a></td><td>
Gets the first line of text.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_MultilineTextAttribute_Line2">Line2</a></td><td>
Gets the second line of text.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_MultilineTextAttribute_Line3">Line3</a></td><td>
Gets third line of text.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_MultilineTextAttribute_Line4">Line4</a></td><td>
Gets the fourth line of text.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_MultilineTextAttribute_Line5">Line5</a></td><td>
Gets the fifth line of text.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.attribute.typeid#System_Attribute_TypeId" target="_blank">TypeId</a></td><td>
When implemented in a derived class, gets a unique identifier for this <a href="https://docs.microsoft.com/dotnet/api/system.attribute" target="_blank">Attribute</a>.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.attribute" target="_blank">Attribute</a>.)</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_MultilineTextAttribute_Value">Value</a></td><td>
Gets the all non-blank lines as string.</td></tr></table>&nbsp;
<a href="#multilinetextattribute-class">Back to Top</a>

## Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="M_CommandLine_Text_MultilineTextAttribute_AddToHelpText">AddToHelpText(HelpText, Boolean)</a></td><td /></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="M_CommandLine_Text_MultilineTextAttribute_AddToHelpText_1">AddToHelpText(HelpText, Func(String, HelpText))</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.attribute.equals#System_Attribute_Equals_System_Object_" target="_blank">Equals</a></td><td>
Returns a value that indicates whether this instance is equal to a specified object.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.attribute" target="_blank">Attribute</a>.)</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.finalize#System_Object_Finalize" target="_blank">Finalize</a></td><td>
Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.attribute.gethashcode#System_Attribute_GetHashCode" target="_blank">GetHashCode</a></td><td>
Returns the hash code for this instance.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.attribute" target="_blank">Attribute</a>.)</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="M_CommandLine_Text_MultilineTextAttribute_GetLastLineWithText">GetLastLineWithText</a></td><td>
Returns the last line with text. Preserves blank lines if user intended by skipping a line.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.gettype#System_Object_GetType" target="_blank">GetType</a></td><td>
Gets the <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a> of the current instance.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.attribute.isdefaultattribute#System_Attribute_IsDefaultAttribute" target="_blank">IsDefaultAttribute</a></td><td>
When overridden in a derived class, indicates whether the value of this instance is the default value for the derived class.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.attribute" target="_blank">Attribute</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.attribute.match#System_Attribute_Match_System_Object_" target="_blank">Match</a></td><td>
When overridden in a derived class, returns a value that indicates whether this instance equals a specified object.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.attribute" target="_blank">Attribute</a>.)</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.memberwiseclone#System_Object_MemberwiseClone" target="_blank">MemberwiseClone</a></td><td>
Creates a shallow copy of the current <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.tostring#System_Object_ToString" target="_blank">ToString</a></td><td>
Returns a string that represents the current object.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr></table>&nbsp;
<a href="#multilinetextattribute-class">Back to Top</a>

## Extension Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_IsEmpty">IsEmpty</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_NormalizeValue">NormalizeValue</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr></table>&nbsp;
<a href="#multilinetextattribute-class">Back to Top</a>

## Explicit Interface Implementations
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Explicit interface implementation](media/pubinterface.gif "Explicit interface implementation")![Private method](media/privmethod.gif "Private method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.attribute.system-runtime-interopservices-_attribute-getidsofnames#System_Attribute_System_Runtime_InteropServices__Attribute_GetIDsOfNames_System_Guid__System_IntPtr_System_UInt32_System_UInt32_System_IntPtr_" target="_blank">_Attribute.GetIDsOfNames</a></td><td>
Maps a set of names to a corresponding set of dispatch identifiers.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.attribute" target="_blank">Attribute</a>.)</td></tr><tr><td>![Explicit interface implementation](media/pubinterface.gif "Explicit interface implementation")![Private method](media/privmethod.gif "Private method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.attribute.system-runtime-interopservices-_attribute-gettypeinfo#System_Attribute_System_Runtime_InteropServices__Attribute_GetTypeInfo_System_UInt32_System_UInt32_System_IntPtr_" target="_blank">_Attribute.GetTypeInfo</a></td><td>
Retrieves the type information for an object, which can be used to get the type information for an interface.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.attribute" target="_blank">Attribute</a>.)</td></tr><tr><td>![Explicit interface implementation](media/pubinterface.gif "Explicit interface implementation")![Private method](media/privmethod.gif "Private method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.attribute.system-runtime-interopservices-_attribute-gettypeinfocount#System_Attribute_System_Runtime_InteropServices__Attribute_GetTypeInfoCount_System_UInt32__" target="_blank">_Attribute.GetTypeInfoCount</a></td><td>
Retrieves the number of type information interfaces that an object provides (either 0 or 1).
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.attribute" target="_blank">Attribute</a>.)</td></tr><tr><td>![Explicit interface implementation](media/pubinterface.gif "Explicit interface implementation")![Private method](media/privmethod.gif "Private method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.attribute.system-runtime-interopservices-_attribute-invoke#System_Attribute_System_Runtime_InteropServices__Attribute_Invoke_System_UInt32_System_Guid__System_UInt32_System_Int16_System_IntPtr_System_IntPtr_System_IntPtr_System_IntPtr_" target="_blank">_Attribute.Invoke</a></td><td>
Provides access to properties and methods exposed by an object.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.attribute" target="_blank">Attribute</a>.)</td></tr></table>&nbsp;
<a href="#multilinetextattribute-class">Back to Top</a>

## See Also


#### Reference
<a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />