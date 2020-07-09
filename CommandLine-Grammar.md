
CommandLineParser Apply GNU stndard in using - or -- as a prefix for options (vs forward slash).

There are two kinds of arguments: Named options and Unbound values:
## Named Options
They are: ShorName and LongName.
### ShorName
 - ShortName begin with a hyphen delimiter ('-').
- Multiple options may follow a hyphen delimiter in a single token if the options do not take arguments (switches or boolean options), i.e they can be merged together. Thus, `-abc` is equivalent to `-a -b -c`.
- Option names are **single** alphanumeric characters, e.g `-a`.
- An option and its argument value may or may not appear as separate tokens. (In other words, the whitespace separating them is optional.) Thus, `-o foo` and `-ofoo` are equivalent.

Short options can be grouped, so that:

```sh
# this is valid (omitting space between short options)
$ myapp -vf my.file

# and also this (omitting space between short option and its value)
$ myapp -vfmy.file
```

For options: ``a``, ``b``, ``c``, ``d``, ``e`` as boolean options and the  ``f`` as scalar string option:

```sh
# this is a valid syntax:
$ myapp -abcdef my.file   # note: that f is the last option 
```

This is not allowed?

```sh
$ myapp -fv my.file # f is scalr option and should be the last, i.e -vf myfile.txt
```

### LongName

- The LongName begin with two dashes, e.g., `--list`.
- The long names are more clear than their corresponding short names. 
- Long options are meant to be obvious and easy to remember, and their meanings are generally easier to discern than those of their corresponding short options. 
- LongName can be merged with its value using `=` separator. Thus,  `--blocking-factor=20` and `--blocking-factor 20` are equivalent.

For example:
 	
```
$ myapp --create --verbose --blocking-factor=20 
```


### Options Terminator DashDash `--`

 - The argument `--` terminates all options; any following arguments are treated as non-option arguments, even if they begin with a hyphen.
 Parser can be configured to accept `--` as option terminator

**Notes:**
- A token consisting of a single hyphen character `-` is interpreted as an ordinary non-option argument. By convention, it is used to specify input from or output to the standard input and output streams (it's allowed in v2.9).

- Options may be supplied in any order, or appear multiple times. The interpretation is left up to the Option Class. 

## Value Options
- They are named Unbound Values.
- Value options are positional arguments and indexed starting 0. 
- They don't begin  with `- or --`.
- Arguments that are precedded by `--` terminator are treated as values even they begin with `- or --`.


## Named Option Types
Named Options are classified to thre types: switches, scalars and sequence options.
### Switch option
- Switch option is a boolean type.
- It's `false` by default.
- If it's passed in the commandline, it will be `true`.
- Switch can be `Nullable<bool>`, and it can be in three state value: `true/ false / null`.

### Example 1:
```cs
// CheckIn = true by default
[Option]
  public bool CheckIn { get; set; }
```
### Example 2: 
Nullable bool
```cs
//set default =true 
[Option(Default = (bool)true)]
public bool? Vsible { get; set; }
```
Commandline arguments:
```
$ myapp --visible false   # Vsible =false
$ myapp --visible true   # Vsible =true
$ myapp    # drop --visible from commandline => Vsible =true (default value)
```
### Scalar option
- Scalar options require one and only one argument value.
- Example: `-a 123`
```cs
[Option("device-name")]
public string DeviceName {get;set;} //scalar
  ```
  Commandline arguments:
  ```
$ myApp --device-name "primary device"  
  ```

### Sequence option
- Sequence  options require one or more argument value.
- its type is: `IEnumerable<T>`
- Option name may be repeated more than one time.
- Thus  `--files file1.txt file2.txt` and   `--files file1.txt   --files file2.txt` are equivalant.

```cs
[Option]
public IEnumerable<string> Files {get;set;} //sequence
```

```
$ myapp --files file1.txt file2.txt
#or
$ myapp --files file1.txt   --files file2.txt   # v2.9+
```

Commandline arguments:
#### Option class sample:
```cs
class Options
{
  [Option ("visible")]
  public bool Visible {get;set;} //switch

  [Option("device-name")]
  public string DeviceName {get;set;} //scalar

  [Option]
  public IEnumerable<string> Files {get;set;} //sequence
  }
```

## See Also:

[[API reference: OptionAttribute|T_CommandLine_OptionAttribute]]
