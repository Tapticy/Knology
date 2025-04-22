
# For loop
What dose this display with out running the code in the compiler?
```c#
for (int i = 0; i < 10; i++)
    {
        Console.WriteLine(i);
        if (i == 7)
            break;
    }

for (int i = 10; i >= 0; i--)
    {
        Console.WriteLine(i);
        if (i == 5)
            break;
    }
```



```c#
for (int i = 0; i < 10; i++)
{
    Console.WriteLine(i);
    if (i == 7)
        break;
}

Console.WriteLine("Press Enter");
Console.ReadLine();
for (int i = 10; i >= 0; i--)
{
    Console.WriteLine(i);
    if (i == 5)
        break;
}
```


# Loop through each element in an array
While the `for` and the `foreach` both iterates through every element
```c#
string[] pick = { "06", "28", "33", "45", "48" };
for (int i = 0; i < pick.Length; i++)
{
    if (pick[i] == "06")
    {
        foreach (string p in pick)
        {
            Console.WriteLine(p);
        }
    }
}
```

# For 
```c#
string a = """
    The Company recognizes the Union as the sole bargaining 
    agent for all employees of the Company at the London Plant except
    supervisors, persons above the rank of supervisor, office, sales staff
    and persons employed for less than twenty-four (24) hours per week.
    """;

string b = """
    Students may be employed for a period not exceeding six months.
    """;

for (int i = 0; i < a.Length; i++)
{
    if (a[i] != b[i])
    {
        foreach (string p in a.Split(' '))
        {
            if (!b.Contains(p))
            {
                Console.WriteLine(p);
            }
        }
        break;
    }
}
```





using random numbers in between `Next(1, 11)`
`monster -= move;` Is decrement any random number like subtracting
`hero += move;` This is increment like adding
```c#
int hero = 0;
int monster = 0;

Random dice = new Random();

/**/
int move = dice.Next(1, 11);
monster -= move;
Console.WriteLine(monster);

hero += move;
Console.WriteLine(hero);
```




```c#
 public static void Main() {

     //int[] draw = [20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30];
     int[] create = new int[11] { 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30 };

     Object[] thisObject = new Object[11] { 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30 };
     Array.Copy(create, thisObject, 2);
 }

 public static void Print(Object[] drawn) {

     foreach (Object i in drawn) {
         Console.Write($"\t{i}");
     }
     Console.WriteLine("");
 }

 public static void Print_One(Object[] drawn) {
     foreach (Object i in drawn) {
         Console.WriteLine($"\t {i}");
     }
     Console.WriteLine("");
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