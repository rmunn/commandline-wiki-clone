Options are rendered in the same order as they appear in the options class.
Options can be reordered using the built-in comparison `RequiredThenAlphaComparison` which reorder options in ascending order based on the longname.

The comparison implement the `Comparison<T> Delegate` as documented [here](https://docs.microsoft.com/en-us/dotnet/api/system.comparison-1?view=netcore-3.1
)

To apply the comparison in custom help, set the `OptionComparison` property as below:

```cs
 h.OptionComparison = HelpText.RequiredThenAlphaComparison;
```

[<img src="media/tryit.png">](https://dotnetfiddle.net/1o3rtH)


Custom comparison can be implemented by implementing `Comparison<T> Delegate`

Custom reordeing by shortname Example:
```cs
static Comparison<ComparableOption> orderOnShortName = (ComparableOption attr1, ComparableOption attr2) =>
    {
    if (attr1.IsOption && attr2.IsOption)
    {
        if (attr1.Required && !attr2.Required)
        {
            return -1;
        }
        else if (!attr1.Required && attr2.Required)
        {
            return 1;
        }
        else
        {
            if (string.IsNullOrEmpty(attr1.ShortName) && !string.IsNullOrEmpty(attr2.ShortName))
            {
                return 1;
            }
            else if (!string.IsNullOrEmpty(attr1.ShortName) && string.IsNullOrEmpty(attr2.ShortName))
            {
                return -1;
            }
            return String.Compare(attr1.ShortName, attr2.ShortName, StringComparison.Ordinal);
        }
    }
    else if (attr1.IsOption && attr2.IsValue)
    {
        return -1;
    }
    else
    {
        return 1;
    }
    };
```

To  use:
```cs
h.OptionComparison = orderOnShortName;
```

[<img src="media/tryit.png">](https://dotnetfiddle.net/1o3rtH)
