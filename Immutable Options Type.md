An immutable class is simply a class whose instances cannot be modified. All of
the information contained in each instance is provided when it is created and is fixed for the lifetime of the object.

Immutable class can work properly if it has: 

- A constructor with parameters.
- The constructor parameters should have the same names as Type properties and in the same order.
- inherited options are expected at the end of the constructor parameter list.
- Constructor Parameters are case-insensitive.

Example:

```cs
class Options {
  private readonly IEnumerable<string> files;
  private readonly bool verbose;
  private readonly long offset;

  public Options(IEnumerable<string> files, bool verbose, long offset) {
    this.files = files;
    this.verbose = verbose;
    this.offset = offset;
  }

  [Option]
  public IEnumerable<string> Files { get { return files; } }

  [Option]
  public bool Verbose { get { return verbose; } }

  [Option]
  public long Offset { get { return offset; } ]
}
```

The previous Options class has the following public properties in order: `Files, Verbose and Offset`

So, the constructor should be:

```cs
//parmeters are in the same order as Properties and have the same name (case-insensitive)
public Options(IEnumerable<string> files, bool verbose, long offset)
```

**Invalid constructors**

```cs
public Options(IEnumerable<string> files, bool verbose)  //less parameters

public Options(long offset, IEnumerable<string> files, bool verbose) //Not match the order of the properties

public Options(IEnumerable<string> files, bool verbose, long offset2) //offset2 has no corresponding property

public Options() //default constructor

```
The Immutable Class without invalid Constructor fire an `InvalidOperationException`:

>Type appears to be immutable, but no constructor found for type `<type name>` to accept values
 

## Immutable Class with Base Class

```cs
class OptionsBase{
public OptionsBase(string name)
	{
		Name=name;
	}
  [Option(Default="xyz")]
  public string Name { get; }
}

class Options: OptionsBase{

//note: name parameter is added as the last parameter 		 
public Options(int testValue, int testValue2,string name):base(name)
{
  //do initialization
}
  [Value(0, MetaName = "Test", Default = 0)]
  public int TestValue { get; }
  [Value(1, MetaName = "Test", Default = 0)]
  public int TestValue2 { get; }
}
		
```

**Note:**

The properties of the Options class should be public. Internal properties are not updated by the Parser.

## Tip
**Save time,  effort and auto create constructor**

This feature will generate constructor, with the proper parameters, automatically. Furthermore, modifying an existing constructor requires updating constructor unless you use this feature to update them automatically.

### Visual studio 2017

Do one of the following:

**Keyboard**

     Press Ctrl+. to trigger the Quick Actions and Refactorings menu.

**Mouse**

- Right-click and select the Quick Actions and Refactorings menu. 
- Click the screwdriver icon that appears in the left margin if the text cursor is already on the empty line in the class. 
- Select Generate constructor from the drop-down menu.

The Pick members dialog box opens.

- Pick all members and Choose OK.

For more details about auto creating constructor, [see](https://docs.microsoft.com/en-us/visualstudio/ide/reference/generate-constructor?view=vs-2019)


### Resharper


     Menu ReSharper | Edit | Generate Code | Constructor

The constructor generation wizard creates a non-default constructor that takes parameters for selected fields, properties and auto-properties.

All generated constructors follow the same pattern where:

Each field, property, or auto-property included in the constructor is initialized with a parameter.

The name of the parameter is derived from the name of the corresponding field or property. 

You can quickly generate constructors by typing ctor (without parameters).

If there are non-default base type constructors, the required parameters are added to the generated constructor and passed to the base class constructor.

For more details about auto creating constructor, [see](https://www.jetbrains.com/help/resharper/Code_Generation__Type_Constructors.html)

### Visual Studio Code

Install `C# Genenate Constructor` extension.

- Press Ctrl+. to trigger the pop-up menu.
- click Generate constructor from properties.

