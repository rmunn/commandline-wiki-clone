# Parser Class
 

Provides methods to parse command line arguments.


## Inheritance Hierarchy
<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br />&nbsp;&nbsp;CommandLine.Parser<br />
**Namespace:**&nbsp;<a href="N_CommandLine">CommandLine</a><br />**Assembly:**&nbsp;CommandLine (in CommandLine.dll) Version: 0.0.0

## Syntax

**C#**<br />
``` C#
public class Parser : IDisposable
```

**VB**<br />
``` VB
Public Class Parser
	Implements IDisposable
```

**C++**<br />
``` C++
public ref class Parser : IDisposable
```

**F#**<br />
``` F#
type Parser =  
    class
        interface IDisposable
    end
```

The Parser type exposes the following members.


## Constructors
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Private method](media/privmethod.gif "Private method")![Static member](media/static.gif "Static member")</td><td><a href="M_CommandLine_Parser__cctor">Parser</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Parser__ctor">Parser()</a></td><td>
Initializes a new instance of the Parser class.</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="M_CommandLine_Parser__ctor_1">Parser(ParserSettings)</a></td><td>
Initializes a new instance of the Parser class</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Parser__ctor_2">Parser(Action(ParserSettings))</a></td><td>
Initializes a new instance of the Parser class, configurable with <a href="T_CommandLine_ParserSettings">ParserSettings</a> using a delegate.</td></tr></table>&nbsp;
<a href="#parser-class">Back to Top</a>

## Properties
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public property](media/pubproperty.gif "Public property")![Static member](media/static.gif "Static member")</td><td><a href="P_CommandLine_Parser_Default">Default</a></td><td>
Gets the singleton instance created with basic defaults.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_CommandLine_Parser_Settings">Settings</a></td><td>
Gets the instance that implements <a href="T_CommandLine_ParserSettings">ParserSettings</a> in use.</td></tr></table>&nbsp;
<a href="#parser-class">Back to Top</a>

## Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Private method](media/privmethod.gif "Private method")![Static member](media/static.gif "Static member")</td><td><a href="M_CommandLine_Parser_DisplayHelp__1">DisplayHelp(T)</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Parser_Dispose">Dispose()</a></td><td>
Frees resources owned by the instance.</td></tr><tr><td>![Private method](media/privmethod.gif "Private method")</td><td><a href="M_CommandLine_Parser_Dispose_1">Dispose(Boolean)</a></td><td>
Releases the unmanaged resources used by the Parser and optionally releases the managed resources</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.equals#System_Object_Equals_System_Object_" target="_blank">Equals</a></td><td>
Determines whether the specified object is equal to the current object.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="M_CommandLine_Parser_Finalize">Finalize</a></td><td>
Finalizes an instance of the Parser class.
 (Overrides <a href="https://docs.microsoft.com/dotnet/api/system.object.finalize#System_Object_Finalize" target="_blank">Object.Finalize()</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.gethashcode#System_Object_GetHashCode" target="_blank">GetHashCode</a></td><td>
Serves as the default hash function.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.gettype#System_Object_GetType" target="_blank">GetType</a></td><td>
Gets the <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a> of the current instance.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Private method](media/privmethod.gif "Private method")![Static member](media/static.gif "Static member")</td><td><a href="M_CommandLine_Parser_HandleUnknownArguments">HandleUnknownArguments</a></td><td /></tr><tr><td>![Private method](media/privmethod.gif "Private method")![Static member](media/static.gif "Static member")</td><td><a href="M_CommandLine_Parser_MakeParserResult__1">MakeParserResult(T)</a></td><td /></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.memberwiseclone#System_Object_MemberwiseClone" target="_blank">MemberwiseClone</a></td><td>
Creates a shallow copy of the current <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Parser_ParseArguments">ParseArguments(IEnumerable(String), Type[])</a></td><td>
Parses a string array of command line arguments for verb commands scenario, constructing the proper instance from the array of types supplied by *types*. Grammar rules are defined decorating public properties with appropriate attributes. The <a href="T_CommandLine_VerbAttribute">VerbAttribute</a> must be applied to types in the array.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Parser_ParseArguments__1">ParseArguments(T)(IEnumerable(String))</a></td><td>
Parses a string array of command line arguments constructing values in an instance of type *T*. Grammar rules are defined decorating public properties with appropriate attributes.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_CommandLine_Parser_ParseArguments__1_1">ParseArguments(T)(Func(T), IEnumerable(String))</a></td><td>
Parses a string array of command line arguments constructing values in an instance of type *T*. Grammar rules are defined decorating public properties with appropriate attributes.</td></tr><tr><td>![Private method](media/privmethod.gif "Private method")![Static member](media/static.gif "Static member")</td><td><a href="M_CommandLine_Parser_Tokenize">Tokenize</a></td><td /></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.tostring#System_Object_ToString" target="_blank">ToString</a></td><td>
Returns a string that represents the current object.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr></table>&nbsp;
<a href="#parser-class">Back to Top</a>

## Extension Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_FormatCommandLine__1">FormatCommandLine(T)(T)</a></td><td>Overloaded.  
Format a command line argument string from a parsed instance.
 (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_FormatCommandLine__1_1">FormatCommandLine(T)(T, Action(UnParserSettings))</a></td><td>Overloaded.  
Format a command line argument string from a parsed instance.
 (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_IsEmpty">IsEmpty</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr><tr><td>![Private Extension Method](media/privextension.gif "Private Extension Method")</td><td><a href="M_CommandLine_UnParserExtensions_NormalizeValue">NormalizeValue</a></td><td> (Defined by <a href="T_CommandLine_UnParserExtensions">UnParserExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CommandLine_ParserExtensions_ParseArguments__10">ParseArguments(T1, T2, T3, T4, T5, T6, T7, T8, T9, T10)(IEnumerable(String))</a></td><td>Overloaded.  
Parses a string array of command line arguments for verb commands scenario, constructing the proper instance from types as generic arguments. Grammar rules are defined decorating public properties with appropriate attributes. The <a href="T_CommandLine_VerbAttribute">VerbAttribute</a> must be applied to types in the array.
 (Defined by <a href="T_CommandLine_ParserExtensions">ParserExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CommandLine_ParserExtensions_ParseArguments__11">ParseArguments(T1, T2, T3, T4, T5, T6, T7, T8, T9, T10, T11)(IEnumerable(String))</a></td><td>Overloaded.  
Parses a string array of command line arguments for verb commands scenario, constructing the proper instance from types as generic arguments. Grammar rules are defined decorating public properties with appropriate attributes. The <a href="T_CommandLine_VerbAttribute">VerbAttribute</a> must be applied to types in the array.
 (Defined by <a href="T_CommandLine_ParserExtensions">ParserExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CommandLine_ParserExtensions_ParseArguments__12">ParseArguments(T1, T2, T3, T4, T5, T6, T7, T8, T9, T10, T11, T12)(IEnumerable(String))</a></td><td>Overloaded.  
Parses a string array of command line arguments for verb commands scenario, constructing the proper instance from types as generic arguments. Grammar rules are defined decorating public properties with appropriate attributes. The <a href="T_CommandLine_VerbAttribute">VerbAttribute</a> must be applied to types in the array.
 (Defined by <a href="T_CommandLine_ParserExtensions">ParserExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CommandLine_ParserExtensions_ParseArguments__13">ParseArguments(T1, T2, T3, T4, T5, T6, T7, T8, T9, T10, T11, T12, T13)(IEnumerable(String))</a></td><td>Overloaded.  
Parses a string array of command line arguments for verb commands scenario, constructing the proper instance from types as generic arguments. Grammar rules are defined decorating public properties with appropriate attributes. The <a href="T_CommandLine_VerbAttribute">VerbAttribute</a> must be applied to types in the array.
 (Defined by <a href="T_CommandLine_ParserExtensions">ParserExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CommandLine_ParserExtensions_ParseArguments__14">ParseArguments(T1, T2, T3, T4, T5, T6, T7, T8, T9, T10, T11, T12, T13, T14)(IEnumerable(String))</a></td><td>Overloaded.  
Parses a string array of command line arguments for verb commands scenario, constructing the proper instance from types as generic arguments. Grammar rules are defined decorating public properties with appropriate attributes. The <a href="T_CommandLine_VerbAttribute">VerbAttribute</a> must be applied to types in the array.
 (Defined by <a href="T_CommandLine_ParserExtensions">ParserExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CommandLine_ParserExtensions_ParseArguments__15">ParseArguments(T1, T2, T3, T4, T5, T6, T7, T8, T9, T10, T11, T12, T13, T14, T15)(IEnumerable(String))</a></td><td>Overloaded.  
Parses a string array of command line arguments for verb commands scenario, constructing the proper instance from types as generic arguments. Grammar rules are defined decorating public properties with appropriate attributes. The <a href="T_CommandLine_VerbAttribute">VerbAttribute</a> must be applied to types in the array.
 (Defined by <a href="T_CommandLine_ParserExtensions">ParserExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CommandLine_ParserExtensions_ParseArguments__16">ParseArguments(T1, T2, T3, T4, T5, T6, T7, T8, T9, T10, T11, T12, T13, T14, T15, T16)(IEnumerable(String))</a></td><td>Overloaded.  
Parses a string array of command line arguments for verb commands scenario, constructing the proper instance from types as generic arguments. Grammar rules are defined decorating public properties with appropriate attributes. The <a href="T_CommandLine_VerbAttribute">VerbAttribute</a> must be applied to types in the array.
 (Defined by <a href="T_CommandLine_ParserExtensions">ParserExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CommandLine_ParserExtensions_ParseArguments__2">ParseArguments(T1, T2)(IEnumerable(String))</a></td><td>Overloaded.  
Parses a string array of command line arguments for verb commands scenario, constructing the proper instance from types as generic arguments. Grammar rules are defined decorating public properties with appropriate attributes. The <a href="T_CommandLine_VerbAttribute">VerbAttribute</a> must be applied to types in the array.
 (Defined by <a href="T_CommandLine_ParserExtensions">ParserExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CommandLine_ParserExtensions_ParseArguments__3">ParseArguments(T1, T2, T3)(IEnumerable(String))</a></td><td>Overloaded.  
Parses a string array of command line arguments for verb commands scenario, constructing the proper instance from types as generic arguments. Grammar rules are defined decorating public properties with appropriate attributes. The <a href="T_CommandLine_VerbAttribute">VerbAttribute</a> must be applied to types in the array.
 (Defined by <a href="T_CommandLine_ParserExtensions">ParserExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CommandLine_ParserExtensions_ParseArguments__4">ParseArguments(T1, T2, T3, T4)(IEnumerable(String))</a></td><td>Overloaded.  
Parses a string array of command line arguments for verb commands scenario, constructing the proper instance from types as generic arguments. Grammar rules are defined decorating public properties with appropriate attributes. The <a href="T_CommandLine_VerbAttribute">VerbAttribute</a> must be applied to types in the array.
 (Defined by <a href="T_CommandLine_ParserExtensions">ParserExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CommandLine_ParserExtensions_ParseArguments__5">ParseArguments(T1, T2, T3, T4, T5)(IEnumerable(String))</a></td><td>Overloaded.  
Parses a string array of command line arguments for verb commands scenario, constructing the proper instance from types as generic arguments. Grammar rules are defined decorating public properties with appropriate attributes. The <a href="T_CommandLine_VerbAttribute">VerbAttribute</a> must be applied to types in the array.
 (Defined by <a href="T_CommandLine_ParserExtensions">ParserExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CommandLine_ParserExtensions_ParseArguments__6">ParseArguments(T1, T2, T3, T4, T5, T6)(IEnumerable(String))</a></td><td>Overloaded.  
Parses a string array of command line arguments for verb commands scenario, constructing the proper instance from types as generic arguments. Grammar rules are defined decorating public properties with appropriate attributes. The <a href="T_CommandLine_VerbAttribute">VerbAttribute</a> must be applied to types in the array.
 (Defined by <a href="T_CommandLine_ParserExtensions">ParserExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CommandLine_ParserExtensions_ParseArguments__7">ParseArguments(T1, T2, T3, T4, T5, T6, T7)(IEnumerable(String))</a></td><td>Overloaded.  
Parses a string array of command line arguments for verb commands scenario, constructing the proper instance from types as generic arguments. Grammar rules are defined decorating public properties with appropriate attributes. The <a href="T_CommandLine_VerbAttribute">VerbAttribute</a> must be applied to types in the array.
 (Defined by <a href="T_CommandLine_ParserExtensions">ParserExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CommandLine_ParserExtensions_ParseArguments__8">ParseArguments(T1, T2, T3, T4, T5, T6, T7, T8)(IEnumerable(String))</a></td><td>Overloaded.  
Parses a string array of command line arguments for verb commands scenario, constructing the proper instance from types as generic arguments. Grammar rules are defined decorating public properties with appropriate attributes. The <a href="T_CommandLine_VerbAttribute">VerbAttribute</a> must be applied to types in the array.
 (Defined by <a href="T_CommandLine_ParserExtensions">ParserExtensions</a>.)</td></tr><tr><td>![Public Extension Method](media/pubextension.gif "Public Extension Method")</td><td><a href="M_CommandLine_ParserExtensions_ParseArguments__9">ParseArguments(T1, T2, T3, T4, T5, T6, T7, T8, T9)(IEnumerable(String))</a></td><td>Overloaded.  
Parses a string array of command line arguments for verb commands scenario, constructing the proper instance from types as generic arguments. Grammar rules are defined decorating public properties with appropriate attributes. The <a href="T_CommandLine_VerbAttribute">VerbAttribute</a> must be applied to types in the array.
 (Defined by <a href="T_CommandLine_ParserExtensions">ParserExtensions</a>.)</td></tr></table>&nbsp;
<a href="#parser-class">Back to Top</a>

## See Also


#### Reference
<a href="N_CommandLine">CommandLine Namespace</a><br />