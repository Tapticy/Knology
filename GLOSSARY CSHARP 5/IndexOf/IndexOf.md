
# IndexOf 
Add code to retrieve the value between parenthesis
```c#
string intro = "CLR: Common Language Runtime (CTS: Common Type)";
int opening = intro.IndexOf('(');
int closing = intro.IndexOf(')');

//Console.WriteLine(intro);   
//Console.WriteLine(opening);

int length = opening - closing;
Console.WriteLine(length);
//-17

int _length = closing - opening;
Console.WriteLine(_length);
//17

Console.WriteLine(intro.Substring(opening, _length));
//  (CTS: Common Type
```

# Modify The String Position Of The Sub String
By increasing the `opening` by `1`, you skip over the opening parenthesis character.
```c#
string intro = "CLR: Common Language Runtime (CTS: Common Type)";
int opening = intro.IndexOf('(');
int closing = intro.IndexOf(')');

opening += 1;
int length = closing - opening;
Console.WriteLine(intro.Substring(opening, length));
// CTS: Common Type

opening += 6;
int _length = closing - opening;
Console.WriteLine(intro.Substring(opening, _length));
// ommon Type
```

The preceding snippet of code shows how to find the value inside an opening and closing <span> tag.
In this case, you're adding 6 to the `opening` as the offset to calculate the length of the sub string.
```c#
string intro = "CLR: Common Language Runtime <span>CTS: Common Type</span>";
// Not a good practice to hard code the IndexOf("<span>")
int opening = intro.IndexOf("<span>");
int closing = intro.IndexOf("</span>");


opening += 6;
int length = closing - opening;
Console.WriteLine(intro.Substring(opening, length));
```

# THIS IS A BETTER PRACTICE 
```c#
string intro = "CLR: Common Language Runtime <span>CTS: Common Type</span>";

const string openSpan = "<span>";
const string closeSpan = "</span>";

int opening = intro.IndexOf(openSpan);
int closing = intro.IndexOf(closeSpan);

opening += openSpan.Length;
int _length = closing - opening;
Console.WriteLine(intro.Substring(opening, _length));
```


```c#
string intro = "PFA: Perform File Operations";

int _first = intro.IndexOf('P');
int _last = intro.LastIndexOf('s');

Console.WriteLine(intro);
Console.WriteLine(_first);
Console.WriteLine(_last);
```

```c#
string message = "(What if) I am (only interested) in the last (set of parentheses)?";
int openingPosition = message.LastIndexOf('(');

openingPosition += 1;
int closingPosition = message.LastIndexOf(')');
int length = closingPosition - openingPosition;
Console.WriteLine(message.Substring(openingPosition, length));
```

# How many time will the loop through ?
```c#
 string message = "(01 03) 04 (05 15) 17 21 (66 9) 23 (34 23) 09";
 while (true) {
     int openingPosition = message.IndexOf('(');
     if (openingPosition == -1) break;

     openingPosition += 1;
     int closingPosition = message.IndexOf(')');
     int length = closingPosition - openingPosition;
     Console.WriteLine(message.Substring(openingPosition, length));
     
     // Note the overload of the Substring to return only the remaining 
     // unprocessed message:
     message = message.Substring(closingPosition + 1);

     /*
      01 03
      05 15
      66 9
      34 23
      */
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