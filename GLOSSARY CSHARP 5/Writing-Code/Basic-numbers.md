
# Increment and decrement
```c#
int value = 0;     // value is now 0.
value = value + 5; // value is now 5.
value += 5;        // value is now 10.

```
## Operators
Operators like `+=, -=, *=, ++,` and `--` are known as compound assignment operators because they compound some operation in addition to assigning the result to the variable. The `+=` operator is specifically termed the addition assignment operator.
```c#
int value = 1;

value = value + 1;
Console.WriteLine("First increment: " + value);

value += 1;
Console.WriteLine("Second increment: " + value);

value++;
Console.WriteLine("Third increment: " + value);

value = value - 1;
Console.WriteLine("First decrement: " + value);

value -= 1;
Console.WriteLine("Second decrement: " + value);

value--;
Console.WriteLine("Third decrement: " + value);
```

This increments 1 `value++`
This increments 2 `++value`
```c#
int value = 1;
value++;
Console.WriteLine("First: " + value);
Console.WriteLine($"Second: {value++}");
Console.WriteLine("Third: " + value);
Console.WriteLine("Fourth: " + (++value));
```


# Create variables to store the sum
```c#
int currentAssignments = 5;

int sophia1 = 93;
int sophia2 = 87;
int sophia3 = 98;
int sophia4 = 95;
int sophia5 = 100;

Console.WriteLine(sophia5 / currentAssignments);

int nicolas1 = 80;
int nicolas2 = 83;
int nicolas3 = 82;
int nicolas4 = 88;
int nicolas5 = 85;

int zahirah1 = 84;
int zahirah2 = 96;
int zahirah3 = 73;
int zahirah4 = 85;
int zahirah5 = 79;

int jeong1 = 90;
int jeong2 = 92;
int jeong3 = 98;
int jeong4 = 100;
int jeong5 = 97;

```



```c#
int sophiaSum = 0;
int nicolasSum = 0;
int zahirahSum = 0;
int jeongSum = 0;

Console.WriteLine("Sophia: "+ ++sophiaSum);
Console.WriteLine("Nicolas: " + nicolasSum);
Console.WriteLine("Zahirah: " + zahirahSum);
Console.WriteLine("Jeong: " + jeongSum);
```

```c#
double a = 1.3;
System.Double b = 12.3;

Console.WriteLine(a);
Console.WriteLine(b);
```


```c#
// assign values to variables - graded assignments 

// decimal sophiaScore;
// decimal nicolasScore;
// decimal zahirahScore;
// decimal jeongScore;

int currentAssignments = 3;
decimal nicolasSum = 0;
decimal zahirahSum = 0;
decimal jeongSum = 0;

decimal nicolasScore = nicolasSum / currentAssignments;
decimal zahirahScore = zahirahSum / currentAssignments;
decimal jeongScore = jeongSum / currentAssignments;
```