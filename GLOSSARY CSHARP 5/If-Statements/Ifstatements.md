
# 
```c#
string name = "steve";

if (name == "bob")
    Console.WriteLine("Found Bob");
else if (name == "steve")
    Console.WriteLine("Found Steve");
else
    Console.WriteLine("Found Chuck Duck");
```

# If Statement Using preprocessing directives
`#if DEBUG` This processes source code before it runs thought the compiler. Strips out all comments replacing it with single space.

```c#
#if DEBUG
void Report(double temp)
{
    if (temp < 20.0) {
        Console.WriteLine("Cold");
    }
    else {
        Console.WriteLine("Hotter");
    }
}
Measurement(200);
Report(12.0);

void Measurement(double value)
{
    if (value <= 20 || value > 100) {
        Console.WriteLine("Not accepted");
    }
    Console.WriteLine($"Measurement is{value}");
}
#endif
```

#
```c#
   var Defined = (CLR: "Common Language Runtime", CTS: "Common Type System");
   var tuple = (age, name);
   tuple.age = 33;
   tuple.name = 3;

   if (tuple.age == 23) {
       Defined.CLR.ToLower();
       Console.WriteLine(Defined.CLR);
   }
   else if (tuple.name == 3) {
       Defined.CTS.ToLower();
       Console.WriteLine(Defined.CTS);
   }
   else {
       Console.WriteLine("not here");
   }
```

# Admin Manger
Created a permission for `Admin|Manger`, if that contains `if (permission.Contains("Admin") )`, and if the level is more than 55 write to the console `Welcome Super Admin User` 
```c#
string permission = "Admin|Manger";

int level = 55;

if (permission.Contains("Admin") ) {
    
    if (level > 55) {
        Console.WriteLine("Welcome Super Admin User");
    }
    else {
        Console.WriteLine("Welcome, Admin User");
    }
}
else if (permission.Contains("Manger")) {
    if (level >= 20) {
        Console.WriteLine("Contact an Admin for access");
    }
    else {
        Console.WriteLine("You do not have sufficient privileges");
    }
}
else {
    Console.WriteLine("privileges is just a word");
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

