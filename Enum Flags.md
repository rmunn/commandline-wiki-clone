
FlagsAttribute in Enum Indicates that an enumeration can be treated as a bit field; that is, a set of flags.
The FlagsAttribute custom attribute is used for an enumeration only if a bitwise operation (AND, OR, EXCLUSIVE OR) is to be performed on a numeric value.

Enumeration is defined as  constants in powers of two, that is, 1, 2, 4, 8, and so on. This means the individual flags in combined enumeration constants do not overlap.

**Remark:** Enum Flags are supported in v2.9+

### Example

```cs
    [Flags]
    enum TestFlagEnum
    {
        None   = 0x0,
        ValueA = 0x1,
        ValueB = 0x2,
        ValueC = 0x4,
        ValueD = 0x8
    }
```

### How to pass enum values on the commandLine
Values should be separated by comma with/o space.
You should quote values in case of using comma and space(s)
#### Valid values
```
 $ myprog --p1 ValueA,ValueB
 $ myprog --p1 "ValueA,   ValueB"
``` 

#### Invalid values
```
 $ myprog --p1 ValueA ValueB        #should be seaprated by comma
 $ myprog --p1 "ValueA   ValueB"    # should be seaprated by comma
``` 

Values can be case insensetive if the parser is configured to accept CaseInsensitiveEnumValues

### Example:
```cs
 var parser = new Parser(with =>
        {
            //ignore case for enum values
            with.CaseInsensitiveEnumValues = true;
        });
```	
#### Valid values
```
 $ myprog --p1 valuea,valueb
 $ myprog --p1 "valuea,   valueb"
 ``` 

Integer values can be passed in the commandline if the values are in range


#### Valid values
```
 $ myprog --p1  3      #valuea,valueb
 $ myprog --p1  4      #ValueC |4
 $ myprog --p1  7      #ValueA, ValueB, ValueC |7
``` 

If values are not in the range, the Parser fail with error `BadFormatConversionError`

## Complete Demo Example

<details>
  <summary>Click to expand!</summary>

```cs

using System;
using System.Collections.Generic;
using CommandLine;

class FlagsDemo
{
  public static void Main()
  {
    //enum values should be separated by comma
  //It can be case insensetive values if parser is configured
    Start("--p1 ValueA,ValueB");
    Start("--p1 valuea,valueb"); //case insensetive
    Start("--p1 VALUEA,valueb"); //case insensetive
    Start("--p1 \"valuea valueb\""); //invalid. it should comma separated
    Start("--p1 \"valuea,    valueb\""); //quote values if separated with comma spaces
    Start("--p1 valuea;valueb"); //invalid
    Start("--p1 3");
    Start("--p1 4");
    Start("--p1 7");
  }
  static void Start(string line)
  {
    Console.WriteLine($"args: {line}");
    var args = line.SplitArgs();
    var parser = new Parser(with =>
    {
        //ignore case for enum values
        with.CaseInsensitiveEnumValues = true;
    });
    
    parser.ParseArguments<Options>(args)
      .WithParsed(Run)
      .WithNotParsed(ErrorHandling);
  }

  static void Run(Options opts)
  {
    Console.WriteLine($"Output: {opts.P1} |{(int)opts.P1}");
  }
  static  void ErrorHandling(IEnumerable<Error> errs)
  {
    Console.WriteLine("Fail");

  }
  [Flags]
  enum TestFlagEnum
  {
    None   = 0x0,
    ValueA = 0x1,
    ValueB = 0x2,
    ValueC = 0x4,
    ValueD = 0x8
  }

  class Options
  {
    [Option]
    public TestFlagEnum P1 { get; set; }
  }
}

```
Output result

```
args: --p1 ValueA,ValueB
Output: ValueA, ValueB |3
args: --p1 valuea,valueb
Output: ValueA, ValueB |3
args: --p1 VALUEA,valueb
Output: ValueA, ValueB |3
args: --p1 "valuea valueb"
Fail
args: --p1 "valuea,    valueb"
Output: ValueA, ValueB |3
args: --p1 valuea;valueb
Fail
args: --p1 3
Output: ValueA, ValueB |3
args: --p1 4
Output: ValueC |4
args: --p1 7
Output: ValueA, ValueB, ValueC |7
```

</details>

[<img src="media/tryit.png">](https://dotnetfiddle.net/yblTU5)

