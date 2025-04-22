# Arithmetic Operators * / % + - << >>
```c#
//Prefer
var v = a + (b * c);

//Over
var v = a + b * c;
```

# Binary Operators && || ?? and or
```c#
//Prefer
var v = a || (b && c);

//Over
var v = a || b && c;
```

# Relational Operators < > <= >= is as == !=
```c#
//Prefer
var v = (a < b) == (c > d);

//Over
var v = a < b == c > d;
```

# Other Operators
```c#
//Prefer
var v = a.b.Length;

//Over
var v = (a.b).Length;
```

# Prefer Object Initializer
```c#
//Prefer
var c = new Customer() {
    Age = 21
}

//Over
var c = new Customer() {
    c.Age = 21;
}
```

# Prefer Collection Initializer
```c#
//Prefer
var list = new List<int>{
    1, 2, 3
}

//Over
var list = new List<int>
list.Add(1);
list.Add(2);
list.Add(3);
```

# Simplified Boolean Expressions
```c#
//Prefer
var x = A() && B();


// Over
var x = A() && B() ? true : false;
```

# Switch Expression
```c#
// Prefer
return num switch {
    1 => 1,
    _ => 2,
}


// Over
switch (num) {
    case 1:
      return 1;
    default:
      return 2;
}
```

# Conditional Expression Over If with Assignments
```c#
// Prefer
string x = expr ? "Whats up" : "Girl";


// Over
string s;
if (expr){
    s = "Hi";
}
else {
    s = "Jack";
}
```

# Conditional Expression Over If With Returns
```c#
// Prefer
return expr ? "Hi" : "Fan";

// Over
if (expr){
    s = "Hi";
}
else {
    s = "Jack";
}
```

# Explicit Tuple Name
```c#
// Prefer
(string name, int age) customer = GetCustomer();
var name = customer.name;
var age = customer.age;

// Over
(string name, int age) customer = GetCustomer();
var name = customer.Item1;
var age = customer.Item2;
```


# Inferred Tuple Element Names
```c#
// Prefer
var tuple = (age, name);


// Over
var tuple = (age: age, name: name);
```


# Simple Default Expression
```c#
// Prefer
void DoWork(CancellationToken cancellationToken = default) {}


// Over
void DoWork(CancellationToken cancellationToken = default(CancellationToken)) {}
```


# Expression Body For Constructors
```c#
class Customer
{
    private int Age;

    public Customer(int age){
        Age = age;
    }
}

// On Single Line
class Customer
{
    private int age;

    public Customer(int age) => Age = age;
}
```

# Expression Body For Properties
```c#
class Customer
{
    private int _age;
    public int Age {get { return _age;}}
}


// On a Single line
class Customer
{
    private int _age;
    public int Age => _age;
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