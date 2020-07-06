OptionAttribute  class provides set of properties to enable the Property as a named option having short or long name like.

##Properties##

 
|	Name| 	Description|
|-------|---------------|
|Default |	Gets or sets mapped property default value. |
|Group |	Gets or sets group of  properties, so only atleast one option is required. |
|HelpText |	Gets or sets a short description of this command line option. Usually a sentence summary. |
|Hidden |	Gets or sets a value indicating whether a command line option is visible in the help text. |
| 	LongName |	Gets long name of this command line option. This name is usually a single english word.
| 	Max|	When applied to IEnumerable<T> properties defines the upper range of items. |
| 	MetaValue |	Gets or sets mapped property meta value. Usually an uppercase hint of required value type. |
| 	Min |	When applied to IEnumerable<T> properties defines the lower range of items. |
| 	Required |	Gets or sets a value indicating whether a command line option is required. 
| 	ResourceType |	Gets or sets the Type that contains the resources for HelpText. |
| 	Separator |	When applying attribute to IEnumerable<T> target properties, it allows you to split an argument and consume its content as a sequence.
| 	SetName |	Gets or sets the option's mutually exclusive set name.
| 	ShortName |	Gets a short name of this command line option, made of one character.

## Default

Default Gets or sets mapped property default value. it's Set by the Parser when no optin is passed in the commandLine.

When `Default` is set to null it may be ignored and the default values are set to:
 
 - The IEnumerables are initialized to empty arrays rather than null.
 - All value type ( int, long ... ) can not be null and the Parser set the default values as described in [Default values of C# types](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/default-values)

 
Default property is object type and need to be casted (Unboxing) to an explicit conversion.

Parser may fire an Exception when it can't convert the value to the target type.

The following example show Unboxing the Default Explictly:

```cs
class Options
{
  [Option("port", Default = (ushort)5001)]
  public ushort UshortValue { get; set; }

  [Option(Default=(short)100 )]
  public short ShortValue { get; set; }
	
  [Option( Default = (bool)true)]
  public bool? Vsible { get; set; }
	
  [Option( Default = (double)5001.4)]
  public double DoubleValue { get; set; }

  [Option( Default = (float)401.3)]
  public float FloatValue { get; set; }
}
```

For decimal values, it can not be casted like:
```cs
//this is not allowed
//Compiler Error: CS0182 An attribute argument must be a constant expression, typeof expression or array creation expression of an attribute parameter type	
[Option( Default = (decimal)401.3M)] //Invalid for attribute parameters
public decimal DecimalValue { get; set; }
```

decimal type is not a valid Attribute Parameter (c# language constraint) see [ref](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/language-specification/attributes#attribute-parameter-types).



See Also:

[[API reference: OptionAttribute|T_CommandLine_OptionAttribute]]
