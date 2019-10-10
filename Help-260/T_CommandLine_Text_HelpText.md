# HelpText Class
 


## Inheritance Hierarchy
<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br />&nbsp;&nbsp;CommandLine.Text.HelpText<br />
**Namespace:**&nbsp;<a href="N_CommandLine_Text">CommandLine.Text</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public class HelpText
```

**VB**<br />
``` VB
Public Class HelpText
```

**C++**<br />
``` C++
public ref class HelpText
```

**F#**<br />
``` F#
type HelpText =  class end
```

The HelpText type exposes the following members.


## Constructors
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Private method](media/privmethod.gif "Private method")![Static member](media/static.gif "Static member")</td><td><a href="M_CommandLine_Text_HelpText__cctor">HelpText</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_HelpText__ctor">HelpText()</a></td><td>
Initializes a new instance of the HelpText class.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_HelpText__ctor_4">HelpText(String)</a></td><td>
Initializes a new instance of the HelpText class specifying heading string.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_HelpText__ctor_1">HelpText(SentenceBuilder)</a></td><td>
Initializes a new instance of the HelpText class specifying the sentence builder.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_HelpText__ctor_5">HelpText(String, String)</a></td><td>
Initializes a new instance of the HelpText class specifying heading and copyright strings.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_HelpText__ctor_2">HelpText(SentenceBuilder, String)</a></td><td>
Initializes a new instance of the HelpText class specifying the sentence builder and heading string.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_HelpText__ctor_3">HelpText(SentenceBuilder, String, String)</a></td><td>
Initializes a new instance of the HelpText class specifying heading and copyright strings.</td></tr></table>&nbsp;
<a href="#helptext-class">Back to Top</a>

## Properties
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_HelpText_AddDashesToOption">AddDashesToOption</a></td><td>
Gets or sets a value indicating whether the format of options should contain dashes. It modifies behavior of <a href="M_CommandLine_Text_HelpText_AddOptions__1">AddOptions(T)(ParserResult(T))</a> method.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_HelpText_AddEnumValuesToHelpText">AddEnumValuesToHelpText</a></td><td>
Gets or sets a value indicating whether to add the values of an enum after the description of the specification.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_HelpText_AdditionalNewLineAfterOption">AdditionalNewLineAfterOption</a></td><td>
Gets or sets a value indicating whether to add an additional line after the description of the specification.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_HelpText_AutoHelp">AutoHelp</a></td><td>
Gets or sets a value indicating whether implicit option or verb 'help' should be supported.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_HelpText_AutoVersion">AutoVersion</a></td><td>
Gets or sets a value indicating whether implicit option or verb 'version' should be supported.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_HelpText_Copyright">Copyright</a></td><td>
Gets or sets the copyright string. You can directly assign a <a href="T_CommandLine_Text_CopyrightInfo">CopyrightInfo</a> instance.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_HelpText_Heading">Heading</a></td><td>
Gets or sets the heading string. You can directly assign a <a href="T_CommandLine_Text_HeadingInfo">HeadingInfo</a> instance.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_HelpText_MaximumDisplayWidth">MaximumDisplayWidth</a></td><td>
Gets or sets the maximum width of the display. This determines word wrap when displaying the text.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_HelpText_OptionComparison">OptionComparison</a></td><td /></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Text_HelpText_SentenceBuilder">SentenceBuilder</a></td><td>
Gets the <a href="P_CommandLine_Text_HelpText_SentenceBuilder">SentenceBuilder</a> instance specified in constructor.</td></tr></table>&nbsp;
<a href="#helptext-class">Back to Top</a>

## Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Private method](media/privmethod.gif "Private method")</td><td><a href="M_CommandLine_Text_HelpText_AdaptVerbsToSpecifications">AdaptVerbsToSpecifications</a></td><td /></tr><tr><td>![Private method](media/privmethod.gif "Private method")</td><td><a href="M_CommandLine_Text_HelpText_AddLine">AddLine(StringBuilder, String)</a></td><td /></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")![Static member](media/static.gif "Static member")</td><td><a href="M_CommandLine_Text_HelpText_AddLine_1">AddLine(StringBuilder, String, Int32)</a></td><td /></tr><tr><td>![Private method](media/privmethod.gif "Private method")</td><td><a href="M_CommandLine_Text_HelpText_AddOption">AddOption</a></td><td /></tr><tr><td>![Private method](media/privmethod.gif "Private method")</td><td><a href="M_CommandLine_Text_HelpText_AddOptionName">AddOptionName</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_HelpText_AddOptions__1">AddOptions(T)(ParserResult(T))</a></td><td>
Adds a text block with options usage string.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_HelpText_AddOptions__1_1">AddOptions(T)(Int32, ParserResult(T))</a></td><td>
Adds a text block with options usage string.</td></tr><tr><td>![Private method](media/privmethod.gif "Private method")</td><td><a href="M_CommandLine_Text_HelpText_AddOptionsImpl">AddOptionsImpl</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_HelpText_AddPostOptionsLine">AddPostOptionsLine</a></td><td>
Adds a text line at the bottom, after options usage string.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_HelpText_AddPostOptionsLines">AddPostOptionsLines</a></td><td>
Adds text lines at the bottom, after options usage string.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_HelpText_AddPostOptionsText">AddPostOptionsText</a></td><td>
Adds a text block of lines at the bottom, after options usage string.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_HelpText_AddPreOptionsLine">AddPreOptionsLine(String)</a></td><td>
Adds a text line after copyright and before options usage strings.</td></tr><tr><td>![Private method](media/privmethod.gif "Private method")</td><td><a href="M_CommandLine_Text_HelpText_AddPreOptionsLine_1">AddPreOptionsLine(String, Int32)</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_HelpText_AddPreOptionsLines">AddPreOptionsLines</a></td><td>
Adds text lines after copyright and before options usage strings.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_HelpText_AddPreOptionsText">AddPreOptionsText</a></td><td>
Adds a text block of lines after copyright and before options usage strings.</td></tr><tr><td>![Private method](media/privmethod.gif "Private method")</td><td><a href="M_CommandLine_Text_HelpText_AddValueName">AddValueName</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_HelpText_AddVerbs_1">AddVerbs(Type[])</a></td><td>
Adds a text block with verbs usage string.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_HelpText_AddVerbs">AddVerbs(Int32, Type[])</a></td><td>
Adds a text block with verbs usage string.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CommandLine_Text_HelpText_AutoBuild__1_1">AutoBuild(T)(ParserResult(T), Int32)</a></td><td>
Creates a new instance of the HelpText class, automatically handling verbs or options scenario.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CommandLine_Text_HelpText_AutoBuild__1">AutoBuild(T)(ParserResult(T), Func(HelpText, HelpText), Func(Example, Example), Boolean, Int32)</a></td><td>
Creates a new instance of the HelpText class using common defaults.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CommandLine_Text_HelpText_DefaultParsingErrorsHandler__1">DefaultParsingErrorsHandler(T)</a></td><td>
Supplies a default parsing error handler implementation.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.equals#System_Object_Equals_System_Object_" target="_blank">Equals</a></td><td>
Determines whether the specified object is equal to the current object.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.finalize#System_Object_Finalize" target="_blank">Finalize</a></td><td>
Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Private method](media/privmethod.gif "Private method")![Static member](media/static.gif "Static member")</td><td><a href="M_CommandLine_Text_HelpText_FormatDefaultValue__1">FormatDefaultValue(T)</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.gethashcode#System_Object_GetHashCode" target="_blank">GetHashCode</a></td><td>
Serves as the default hash function.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Private method](media/privmethod.gif "Private method")</td><td><a href="M_CommandLine_Text_HelpText_GetMaxLength">GetMaxLength</a></td><td /></tr><tr><td>![Private method](media/privmethod.gif "Private method")</td><td><a href="M_CommandLine_Text_HelpText_GetMaxOptionLength">GetMaxOptionLength</a></td><td /></tr><tr><td>![Private method](media/privmethod.gif "Private method")</td><td><a href="M_CommandLine_Text_HelpText_GetMaxValueLength">GetMaxValueLength</a></td><td /></tr><tr><td>![Private method](media/privmethod.gif "Private method")</td><td><a href="M_CommandLine_Text_HelpText_GetSpecificationsFromType">GetSpecificationsFromType</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.gettype#System_Object_GetType" target="_blank">GetType</a></td><td>
Gets the <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a> of the current instance.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Private method](media/privmethod.gif "Private method")![Static member](media/static.gif "Static member")</td><td><a href="M_CommandLine_Text_HelpText_GetUsageFromType">GetUsageFromType</a></td><td /></tr><tr><td>![Private method](media/privmethod.gif "Private method")</td><td><a href="M_CommandLine_Text_HelpText_MakeHelpEntry">MakeHelpEntry</a></td><td /></tr><tr><td>![Private method](media/privmethod.gif "Private method")</td><td><a href="M_CommandLine_Text_HelpText_MakeVersionEntry">MakeVersionEntry</a></td><td /></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.memberwiseclone#System_Object_MemberwiseClone" target="_blank">MemberwiseClone</a></td><td>
Creates a shallow copy of the current <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CommandLine_Text_HelpText_RenderParsingErrorsText__1">RenderParsingErrorsText(T)</a></td><td>
Builds a string that contains a parsing error message.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CommandLine_Text_HelpText_RenderParsingErrorsTextAsLines__1">RenderParsingErrorsTextAsLines(T)</a></td><td>
Builds a sequence of string that contains a parsing error message.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CommandLine_Text_HelpText_RenderUsageText__1">RenderUsageText(T)(ParserResult(T))</a></td><td>
Builds a string with usage text block created using <a href="T_CommandLine_Text_UsageAttribute">UsageAttribute</a> data and metadata.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CommandLine_Text_HelpText_RenderUsageText__1_1">RenderUsageText(T)(ParserResult(T), Func(Example, Example))</a></td><td>
Builds a string with usage text block created using <a href="T_CommandLine_Text_UsageAttribute">UsageAttribute</a> data and metadata.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")![Static member](media/static.gif "Static member")</td><td><a href="M_CommandLine_Text_HelpText_RenderUsageTextAsLines__1">RenderUsageTextAsLines(T)</a></td><td>
Builds a string sequence with usage text block created using <a href="T_CommandLine_Text_UsageAttribute">UsageAttribute</a> data and metadata.</td></tr><tr><td>![Private method](media/privmethod.gif "Private method")</td><td><a href="M_CommandLine_Text_HelpText_ToComparableOption">ToComparableOption</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Text_HelpText_ToString">ToString</a></td><td>
Returns the help screen as a <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>.
 (Overrides <a href="https://docs.microsoft.com/dotnet/api/system.object.tostring#System_Object_ToString" target="_blank">Object.ToString()</a>.)</td></tr></table>&nbsp;
<a href="#helptext-class">Back to Top</a>

## Operators
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public operator](media/puboperator.gif "Public operator")![Static member](media/static.gif "Static member")</td><td><a href="M_CommandLine_Text_HelpText_op_Implicit">Implicit(HelpText to String)</a></td><td>
Converts the help instance to a <a href="https://docs.microsoft.com/dotnet/api/system.string" target="_blank">String</a>.</td></tr></table>&nbsp;
<a href="#helptext-class">Back to Top</a>

## Fields
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public field](media/pubfield.gif "Public field")![Static member](media/static.gif "Static member")</td><td><a href="F_CommandLine_Text_HelpText_RequiredThenAlphaComparison">RequiredThenAlphaComparison</a></td><td /></tr></table>&nbsp;
<a href="#helptext-class">Back to Top</a>

## Extension Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_IsEmpty">IsEmpty</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_NormalizeValue">NormalizeValue</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr></table>&nbsp;
<a href="#helptext-class">Back to Top</a>

## See Also


#### Reference
<a href="N_CommandLine_Text">CommandLine.Text Namespace</a><br />