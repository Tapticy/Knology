
# IDictionary Int String
```c#
class Program
{
    static void Main(string[] args)
    {
        Dictionary<int, string> map = new()
        {
            { 1, "FireWire" },
            { 2, "eSATA" },
            { 3, "USB" },
        };

        foreach (KeyValuePair<int, string> m in map)
        {
            Console.WriteLine($"{m.Key} and {m.Value}");
        }

        Console.WriteLine();
        foreach ((var option, var answer) in map)
        {
            Console.WriteLine($"{option} {answer}");
        }
    }
}
```

# Generics 
Using a while loop is the only way to print to console 
```c#
 Dictionary<int, string> map = new();
 map.Add(1, "CLR");
 map.Add(2, "JIT");
 map.Add(3, "PFA");
 
 while (map.Count > 0) {
     Console.WriteLine(map.Values.First());
     Console.WriteLine(map.Values.Last());
     break;
 }

  
 // or
 Dictionary<int, string> akey = new() {
     {1, "one"},
     {2, "two"},
     {3, "three" }
 };
 for (int i = 0; i < akey.Count; i++) {
     Console.WriteLine(i);
 }

 // 
 Stack<string> stack = new Stack<string>();
 stack.Push("Common Language Runtime");
 stack.Push("Just In Time");
 stack.Push("Perform File Operations");
 foreach (string s in stack) {
     Console.WriteLine(s);
 }
```

# Dictionary 
```c#
class Program
{
    static void Main(string[] args)
    {
        Dictionary<int, string> map = new()
        {
            { 1, "FireWire" },
            { 2, "eSATA" },
            { 3, "USB" },
        };

        Console.WriteLine();
        foreach ((var option, var answer) in map)
        {
            Console.WriteLine($"{option} {answer}");
        }
    }
}
```

# template
```c#
class Program
{
    static void Main(string[] args) { }
}
```

# Counting 0 to 5
```c#
// Count for 0 to 5
for (int i = 0; i < 6; i++)
{
    Console.WriteLine("" + i);
}
```

# Generic List of strings and integer
```c#

List<int> numbers = [10, 13, 24, 35, 38, 45];
foreach (var num in numbers)
{
    Console.WriteLine($"Output \t {num}");
}


List<string> definitions = ["\tA FireWire", "\tB eSATA", "\tC USB"];
foreach (var define in definitions)
{
    Console.WriteLine($"{define}");
}
```

