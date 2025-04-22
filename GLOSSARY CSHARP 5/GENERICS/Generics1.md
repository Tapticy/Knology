 
ATAPI (Advanced Technology Attachment Packet Interface)
An interface standard, part of the IDE/ATA standards, that allows tape drives, optical drives, and other drives to be treated like an IDE hard drive by the system. 


ATX 
The most common form factor for PC systems presently in use, originally introduced by Intel in 1995. ATX motherboards and cases make better use of space and resources than did the earlier AT form factor.

 
ATX12V power supply 
A power supply that provides a 12V power cord with a 4-pin connector to be used by the auxiliary 4-pin power connector on motherboards used to provide extra power for processors. 


# Generics List 
```c#
List<string> glo = ["ATAPI", "ATX", "ATX12V"];

int[] c = new int[glo.Count];

foreach (var ary in glo)
{
    if (ary.StartsWith("ATX"))
    {
        Console.WriteLine(ary);
    }
}

Console.WriteLine(c.Length);
```


# Generics 
## Count First Method
`text.Count` This count is builtin method that counts how meany strings
in the list

`text.First()` -If i use the First() builtin method displays to the Console.
```c#
List<string> text = new();
text.Add("Ammeter");
Console.WriteLine($"There are: {text.Count}");

// First() Method
Console.WriteLine($"There is {text.First()} in this list");
```


# Static Generic Method That I Named
```c#
static void Anonymous<T>(ref T user, ref T answer)
{
    T Question;
    Question = answer;
    answer = user;
    answer = Question;
}

static void Testing()
{
    string a = "answer";
    string b = "question";

    Anonymous<string>(ref a, ref b);
    Console.WriteLine(a + " " + b);
}

Testing();
```

```c#
class Program
{
    static void Main()
    {
        // Create a stack of integers
        Stack<int> intStack = new Stack<int>();

        // Push elements onto the stack
        intStack.Push(1);
        intStack.Push(2);
        intStack.Push(3);

        // Pop elements from the stack
        Console.WriteLine(intStack.Pop()); // Output: 3
        Console.WriteLine(intStack.Pop()); // Output: 2

        // Peek at the top element without removing it
        Console.WriteLine(intStack.Peek()); // Output: 1
    }
}
```