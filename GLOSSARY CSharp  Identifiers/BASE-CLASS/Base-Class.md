
```c#
public class Contact
{
    protected string? number = "";
    protected string? name = "";

    protected int count = 0;

    public virtual void GetInfo()
    {
        count++;
        Console.WriteLine("Enter Name");
        name = Console.ReadLine();
        Console.WriteLine("");
        Console.WriteLine($"Name: {count} {name}");

        Console.WriteLine("Enter Number");
        number = Console.ReadLine();
        Console.WriteLine("");
        Console.WriteLine($"Number: {count} {number}");
    }
}

class Display : Contact
{
    public string id = "ABC4938EFG";

    public override void GetInfo()
    {
        count++;
        base.GetInfo();
        Console.WriteLine($"ID: {count} {id}");
    }
}

class Program
{
    static void Main(string[] args) 
    { 
        Display show = new Display();
        show.GetInfo();
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


```c#
```