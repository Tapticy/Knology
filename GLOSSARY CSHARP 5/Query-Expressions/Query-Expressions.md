
# The From Clause Reference
This data source referenced in the from clause must have a type of `IEnumerable<int>`.
```c#
 List<int> Draw = [18, 19, 20, 22, 27, 44, 48];
 IEnumerable<int> totalWin = from drawn in Draw
                             where drawn < one.Length
                             select drawn;
 foreach (int i in totalWin) {
     Console.Write($"\t {i}\n");
 }
```

A query expression must begin with a from clause, and can 
contain sub-queries which will also begin with a from clause
```c#
int[] one = [01, 03, 04, 05, 15, 17, 21];

var draw = from o in one
            where o < 7 select o;
foreach (int i in draw) {
    Console.Write($"\t{i}");
}
```

Each element in the list contains an inner sequence of scores.
```c#
class Program
{
    public class Student
    {
        // The element type of the data source.
        public required string LastName { get; init; }
        public required List<int> Scores { get; init; }
    }

    static void Main(string[] args) {
        // using a collection initializer to create data source
        List<Student> students = [
            new Student {LastName = "Jackson", Scores = [97, 72, 81, 60]},
            new Student {LastName = "Tennant", Scores = [75, 84, 91, 39]},
            new Student {LastName = "Mortensen", Scores = [88, 94, 65, 85]}
            ];
 
        //Use a compound from to access the inner sequence within each element.
        // Note the similarity to a nested foreach statement
        var scoreQuery = from student in students
                         from score in student.Scores
                         where score > 90
                         select new { Last = student.LastName, score };

        // Execute the queries.
        Console.WriteLine("scoreQuery:");

        // Rest the mouse pointer on scoreQuery in the following line to
        // see its type. The type is IEnumerable<'a>, where 'a is an
        // anonymous type defined as new {string Last, int score}. That is,
        // each instance of this anonymous type has two members, a string
        // (Last) and an int (score).
        foreach (var student in scoreQuery) {
            Console.WriteLine("{0} Score: {1}", student.Last, student.score);
        }
    }
}
```
# output
scoreQuery:
Jackson Score: 97
Tennant Score: 91
Mortensen Score: 94

# From Clause 
```c#
   string[] value = { "12.3", "45", "ABC", "11", "DEF" };
   decimal total = 0m;
   string message = "";

   foreach (var i in value) {
       decimal num;// store Trypars out value
       if (decimal.TryParse(i, out num)) {
           total += num;
       }
       else {
           message += i;
       }
   }
   Console.Write($"Message: {message}");
   Console.WriteLine();
   Console.WriteLine($"Total: {total}");
```

#
```c#
  List<int> drawn = [18, 19, 20, 22, 27, 44, 48];
  IEnumerable<int> total = from d in drawn
                           where d < drawn.Count
                           select d;

  foreach (int t in total) {
      Console.Write($"\t {t}");
  }

  List<string> abb = ["CLR", "CTS", "PFA", "JIT"];
  IEnumerable<string> total2 = from a in abb
                               where a == abb[2]
                               orderby a descending
                               select $"Similar to an if {a}";

  foreach (string t in total2) {
      Console.WriteLine($"{t}");
  }
```

# Numbers 
```c#
  Console.WriteLine();
  List<int> number = [01, 07, 08, 17, 23, 37, 44];
  var hightSomething = (from n in number
                        where n > 44
                        select n).Count();

  foreach (int n in number) {
      Console.Write($"\t{n}");
  }
```

# 
```c#
  string text = """
      The Array.Clear() method enables you to eliminate the contents of specific elements in your array 
      """;
 
  IEnumerable<string> words = from t in text.Split(' ')
                              where t.Length > 0
                              select t;

  foreach (var w in words) {
      Console.WriteLine($"{w}");
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