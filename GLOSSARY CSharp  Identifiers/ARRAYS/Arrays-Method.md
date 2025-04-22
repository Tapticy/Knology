# Discover Sort() and Reverse()
```c#
 string[] pallets = ["B14", "A11", "B12", "A13"];

 Console.WriteLine("Sorted...");
 Array.Sort(pallets);
 foreach (var pallet in pallets) {
     Console.Write($"\t-- {pallet}");
 }
```
# Collection Expressions
```c#
  var one = new int[3] { 1, 2, 3 };
  foreach (var o in one) {
      Console.WriteLine($"1 Array: {o}");
  }

  var two = new int[] { 1, 2, 3, 4 };
  foreach (var t in two) {
      Console.WriteLine($"2 Array: {t}");
  }

  var three = new[] { 1, 2, 3, 4, 5 };
  foreach (var t in three) {
      Console.WriteLine($"{t}");
  }


  int[] four = { 1, 2, 3, 4, 5, 6, 7 };
  foreach (var f in four) {
      Console.WriteLine($"{f}");
  }
```

  All four versions are functionally equivalent, and the compiler generates identical code for each version. The last example is similar to the new collection
  expressions syntax. If you squint your eyes a bit, you could imagine the curly braces as { and } as square brackets [ and ], then you’d be reading the new 
  collection expression syntax. Collection expressions don’t use curly braces. This is to avoid ambiguity with existing syntax, especially { } to indicate 
  any not-null in patterns.


The last example is the only to declare the type explicitly, instead of relying on var. The following example creates aList<char>:
```c#
 List<char> pat = ['P', 'A', 'T'];

 int[] emptyCollection = [];
```

To reverse the order of the pallets using the Array.Reverse() method, update your code as follows:
```c#
string[] pallets = ["B14", "A11", "B12", "A13"];
Console.WriteLine("Sorted...");
Array.Sort(pallets);
foreach (var pallet in pallets) {
    Console.WriteLine($"-- {pallet}");
}


Console.WriteLine("");
Console.WriteLine("Reversed...");
Array.Reverse(pallets);
foreach (var pallet in pallets) {
    Console.WriteLine($"-- {pallet}");
}
```


```c#
 string[,] port = { { "EPS", "AGP" }, { "API", "CDN" } };
 foreach (var p in port) {
     Console.WriteLine(p);
 }

 int[,] numbers = { { 1, 4, 2 }, { 3, 6, 8 } };

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