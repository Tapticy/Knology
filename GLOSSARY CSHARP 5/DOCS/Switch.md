# Switch Statement
Using a `sku` inside a switch statement `type`, `color` and `size`.
So the `string[] product` that is assigned `=` to `sku.Split('-');`,
Splits up string `02-BL-S` with `case "01"`, `case "BL"` and `case "S"`
along with type, color and size. 
```c#
// SKU = Stock Keeping Unit.
// SKU value format: <product #>-<2-letter color code>-<size code>
string sku = "02-BL-S";

string[] product = sku.Split('-');

string type = "";
string color = "";
string size = "";

switch (product[0])
{
    case "01":
        type = "Sweat Shirt";
        break;
    case "02":
        type = "T-Shirt";
        break;
    case "03":
        type = "Sweat Pants";
        break;
    default:
        type = "Another Type";
        break;
}

Console.WriteLine($"Type of material: {type}");

switch (product[1])
{
    case "BL":
        color = "Black";
        break;
    case "MN":
        color = "Maroon";
        break;
    default:
        color = "White";
        break;
}
Console.WriteLine($"Color is: {color}");

switch (product[2])
{
    case "S":
        size = "Small";
        break;
    case "M":
        size = "Medium";
        break;
    case "L":
        size = "Large";
        break;
    default:
        size = "End of Size";
        break;
}

Console.WriteLine($"Size is: {size}");
```



```c#
class Program
{
    static void Main(string[] args)
    {
        // SKU = Stock Keeping Unit.
        // SKU value format: <product #>-<2-letter color code>-<size code>
        string sku = "01-MN-L";

        string[] product = sku.Split('-');

        string type = "";
        string color = "";
        string size = "";

        switch (product[0])
        {
            case "01":
                type = "Sweat Shirt";
                break;
            case "02":
                type = "T-Shirt";
                break;
            case "03":
                type = "Sweat Pants";
                break;
            default:
                type = "Another Type";
                break;
        }

        Console.WriteLine($"Type of material: {type}");

        switch (product[1])
        {
            case "BL":
                color = "Black";
                break;
            case "MN":
                color = "Maroon";
                break;
            default:
                color = "White";
                break;
        }
        Console.WriteLine($"Color is: {color}");

        size = product[2] switch
        {
            "S" => "Small",
            "M" => "Medium",
            "L" => "Large",
            _ => "End of Size",
        };
        Console.WriteLine($"Size is: {size}");
    }
}
```



```c#
string sku = "03-MN-M";

string? type = ""; string? color = ""; string? size = "";
string[] product = sku.Split('-');

try
{
    type = product[0] switch
    {
        "01" => "Sweat Shirt",
        "02" => "T-Shirt",
        "03" => "Pants",
        _ => "End of Size",
    };
    Console.WriteLine($"Material: {type}");

    color = product[1] switch
    {
        "BL" => "black",
        "MN" => "Maroon",
        "RD" => "Red",
        _ => "No More colors",
    };
    Console.WriteLine($"Color is: {color}");

    size = product[2] switch
    {
        "S" => "Small",
        "M" => "Medium",
        "L" => "Large",
        _ => "End of Size",
    };
    Console.WriteLine($"Size is: {size}");

}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}

```

#
```c#
DisplayMeasurements(3, 4); // Output: First measurement is 3, second measurement is 4.
DisplayMeasurements(5, 5); // Output: Both measurements are valid and equal to 5.

void DisplayMeasurements(int a, int b)
{
    switch ((a, b))
    {
        case (> 0, > 0) when a == b:
            Console.WriteLine($"Both measurements are valid and equal to {a}.");
            break;

        case (> 0, > 0):
            Console.WriteLine($"First measurement is {a}, second measurement is {b}.");
            break;

        default:
            Console.WriteLine("One or both measurements are not valid.");
            break;
    }
}
```

```c#
```



```c#
```



```c#
```




```c#
```



```c#
```




```c#
```



```c#
```