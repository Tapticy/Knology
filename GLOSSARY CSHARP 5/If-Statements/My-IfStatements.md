
# Choose The Right Answer
Just a simple question: `"Why is all data stored in a computer in binary form?"`.
With 3 Answers to choose from, 3 string answers and user can pick the right one `string user = Console.ReadLine();`:

`string one = "1. Numbers are given away then data is available.";`

`string two = "2. Grouping is often done in groups of eight bits.";`

`string three = "3. Colors can be numbers in grouping graphics.";`

And the user gets 10 points `points += 10;` if 2 is picked, by the using the contains method `user.Contains("2") == two.Contains("2")`. If you look between
`user.Contains()` this `.` is called an operator.
And the `int`, `string` are Access-Modifiers Data Types.   
```c#
int points = 0;
string one = "1. Numbers are given away then data is available.";
string two = "2. Grouping is often done in groups of eight bits.";
string three = "3. Colors can be numbers in grouping graphics.";

Console.WriteLine("Why is all data stored in a computer in binary form?");
Console.WriteLine();
Console.Write($"\t{one}\n");
Console.Write($"\t{two}\n");
Console.Write($"\t{three}\n");
#nullable disable
string user = Console.ReadLine();

if (user.Contains("2") == two.Contains("2")) {
    points += 10;
    Console.WriteLine($"That is correct: {two} you get {points} Points");
}
else if (user.Contains("1") == one.Contains("1")) {
    Console.WriteLine($"Not-right: {one}");
}
else if (user.Contains("3") == three.Contains("3")) {
    Console.WriteLine($"Not-Right: {three}");
}
else {
    Console.WriteLine("Pick the correct One");
}
``

# Comparing 
Comparing user value to an array of numbers
```c#
 int[] draw1 = [24, 43, 45, 47, 49];
 int[] pick1 = new int[5];

 string use = Convert.ToString(pick1);
 Console.WriteLine("Enter");
 use = Console.ReadLine();
 if (use == "24") {
     Console.WriteLine($"24 is first\n");
     foreach (int i in draw1) {
         Console.Write($"\t{i}");
     }
 }
 else if (use == "43") {
     Console.WriteLine("43 is second\n");
     foreach (int i in draw1) {
         Console.Write($"\t{i}");
     }
 }
 else if (use == "45") {
     Console.WriteLine("45 is Third\n");
     foreach (int i in draw1) {
         Console.Write($"\t{i}");
     }
 }
 else if (use == "47") {
     Console.WriteLine("47 is Fourth\n");
     foreach (int i in draw1) {
         Console.Write($"\t{i}");
     }
 }
 else if (use == "49") {
     Console.WriteLine("49 is Fifth\n");
     foreach (int i in draw1) {
         Console.Write($"\t{i}");
     }
 }
 else {
     Console.WriteLine("Not one number here\n");
     foreach (int i in draw1) {
         Console.Write($"\t{i}");
     }
 }
``

```c#
``

```c#
``

```c#
``

```c#
``

```c#
``

```c#
``


```c#
``

```c#
``

```c#
``

```c#
``


```c#
``

```c#
``

```c#
``

```c#
``


```c#
``

```c#
``

```c#
``

```c#
``



```c#
``

```c#
``

```c#
``

```c#
``



```c#
``

```c#
``

```c#
``

```c#
``



```c#
``

```c#
``

```c#
``

```c#
``


```c#
``

```c#
``

```c#
``

```c#
``