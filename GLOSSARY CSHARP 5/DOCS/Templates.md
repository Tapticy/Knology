# Class Main Program Template

```c#
class Program
{
    static void Main(string[] args)
    {
        
    }
}
```

# Switch

```c#
switch (text)
{
    case "":
        Console.WriteLine($"");
        break;

    case "":
        Console.WriteLine($"");
        break;
            
    case "":
        Console.WriteLine($"");
        break;
}
```

# Array Template

```c#
string[] firstNames = { "", "", "", "" };
Console.WriteLine("1 Entry");
firstNames[0] = Console.ReadLine();
Console.WriteLine("2 Entry");
firstNames[1] = Console.ReadLine();
Console.WriteLine("3 Entry");
firstNames[2] = Console.ReadLine();
Console.WriteLine("4 Entry");
firstNames[3] = Console.ReadLine();
Console.WriteLine("");
Console.WriteLine($"Saved: {firstNames.ToList()}");
```

# For loop Template

```c#
string[] names = { "", "", "", "" };

for (int i = 0; i < names.Length; i++)
{
    if (names[i] == "")
    {
        names[i] = "";
    }
}

foreach (var name in names)
{
    Console.WriteLine(name);
}

Console.ReadLine();
for (int i = 0; i < 20; i++)
{
    Console.WriteLine(i);
}
```

# For Template

```c#
for (int i = 0; i < 20; i++)
{
    switch (i)
    {
        case 0:
            // variable assignments were removed for this view of the structure
            break;

        case 1:
            // variable assignments were removed for this view of the structure
            break;

        case 2:
            // variable assignments were removed for this view of the structure
            break;

        case 3:
            // variable assignments were removed for this view of the structure
            break;

        default:
            // variable assignments were removed for this view of the structure
            break;
    }
}

```

# Switch

```c#
switch()
{
    case "1":
        break;

    case "2":
        break;

    case "3":
        break;

    case "4":
        break;

    case "5":
        break;

    case "6":
        break;

    case "7":
        break;

    case "8":
        break;

}
```

```c#
string[]? select = { "", "" };
string[] from = { "", "" };
string[] where = { "", "" };
string[] groupBy = { "", "" };
string[] having = { "", "" };
string[] orderBy = { "", "" };
string[] limit = { "", "" };

int counting = 0;

// bool isSelect = false;

string line = "variable assignments were removed for this view of the structure";
Console.WriteLine(line + "\n");

Console.WriteLine("Enter v to count the letter");
select[0] = Console.ReadLine();
char[] lookIn = line.ToCharArray();

foreach (char c in lookIn)
{
    if (select[0].Contains("v"))
    {
        if (c == 'v')
        {
            counting++;
        }
    }
}
Console.WriteLine($"The number of 'v' in the string is: {counting}");

```

```c#
```

```c#
```

```c#
```

```c#
```
