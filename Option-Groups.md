You can define options as belonging to a group. An option group represents a group of options which are optional, but at least one should be available.
You can provide values to all options in a group. If none of the options belonging to a group have value, you will get an error.

You can define more than one option group.

> NOTE: Required rules are ignored if an option belongs to an option group. If an options is marked as `Required`, it will not be treated as required and the `Required` label will not appear in help text.

Group options in different option groip by defining the options class as follows:

``` csharp
class AppendToFileNameOptions
{
    //define commands in set(group) named fetch
  [Option(Group = "append", HelpText="Prefix to append to file name")]
  public string Prefix { get; set; }

  [Option(Group  = "append", HelpText="Suffix to append to file name")]
  public string Suffix { get; set; }

  [Option("source", HelpText="The path of a file to rename")]
  public string FilePath { get; set; }
}
```

<!-- Put proper demo -->
<!-- [<img src="media/tryit.png">](https://dotnetfiddle.net/GeXOFY) -->

# Examples

```
myapp --source C:\test\file.txt --prefix "test-" --suffix "-2019"
```

```
myapp --source C:\test\file.txt --prefix "test-"
```

```
myapp --source C:\test\file.txt --suffix "-2019"
```

## Error scenario
```
myapp --source C:\test\file.txt
```

This will produce `MissingGroupOptionError` containing the group name and the option names which belong to this group

# Help text

Consider the options scenario above. Group name will be rendered as part of the help text before the option help text

```
Myapp 2.0.0-beta
Copyright (c) 2019 Global.com

  --source Required. The path of a file to rename
  --prefix (Group: append) Prefix to append to file name
  --suffix (Group: append) Suffix to append to file name
```