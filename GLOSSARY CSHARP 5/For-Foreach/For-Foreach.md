# The Difference Between Do and While statement iterations
# For Loop
```c#
for (int i = 1; i < 101; i++)
{
    if ((i % 3 == 0) && (i % 5 == 0))
    {
        Console.WriteLine($"{i} - FizzBuzz");
    }
    else if (i % 3 == 0)
    {
        Console.WriteLine($"{i} i Fizz");
    }
    else if (i % 5 == 0)
    {
        Console.WriteLine($"{i} i Buzz");
    }
    else
    {
        Console.WriteLine($"{i}");
    }
}
```




# String and For loop
```c#
 string[] just = ["T", "Y", "P", "E"];

 for (int i = 0; i < just.Length; ++i) {
     if (just[i] == "E") {
         foreach (string d in just) {
             Console.WriteLine(d);
         }
     }
 }

```

# Letters looping through a foreach
```c#
 string[] letters = { "A", "B", "C" };
 char[] Letters = { 'D', 'E', 'F' };
 
 foreach (string l in letters) {
     Console.WriteLine($"{l}");
 }

 foreach (char L in Letters) {
     Console.WriteLine($"{L}");
 }
```

# Array.Sort() Method
```c#
int[] num = { 1, 2, 3 };
int[] pta = new int[num.Length];
Array.Sort(num, pta);
foreach (int i in pta) {
    Console.Write($"{i}");
}
```
## OutPut
 000



# System Linq 
Array Methods `Max` `Min` or `Sum`
```c#
int[] num = { 5, 2, 9, 1, 6, 9 };
Console.Write($"{num.Max()}");
Console.Write($"{num.Min()}");
Console.Write($"{num.Sum(x => x)}");
```
## OutPut
9132


# Sort() Method
```c#
 string[] port = { "EPS", "API", "AGP", "CDN" };
 Array.Sort(port);
 foreach (string p in port) {
     Console.Write($"\t{p}");
 }
```

### Table Visualization In Mind
# Multidimensional Arrays
2 Dimensional Arrays with a single comma `[,]`
3 Dimensional Arrays have 2 commas `[,,]`
First Row `{ 3, 9, 5 }` with 3 columns in this row
Second Row `{ 4, 5, 6 }` with 3 columns in this row

```c# 
int[,] dimensional2 = { { 3, 9, 5 }, { 4, 7, 6 } };

// first row 0  third column 2
Console.Write($"\t{dimensional2[0, 2]}");
Console.Write($"\t{dimensional2[1, 2]}");
Console.Write($"\t{dimensional2[1, 1]}");
```

## Changing Values In a String 2D Array
```c#
string[,] port = { { "EPS", "AGP" }, { "API", "CDN" } };
port[0, 0] = "PAT";
Console.WriteLine(port[0, 0]);
```

# Looping Through 
Looping an array called bingo
```c#
string[] bingo = ["B", "I", "N", "G", "O"];
int[] drawn = [2, 4, 12, 9, 10];

foreach (var b in bingo) {
    Console.Write($"\t{b}");
}
Console.WriteLine();
for (int i = 0; i < drawn.Length i++) {
    Console.Write($"\t{i}");
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