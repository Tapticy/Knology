
# Creating Methods
```c#
int[] selection = new int[1];
bool[] correct = new bool[1];
double[] score = new double[1];

// Welcome void Method
void Welcome()
{
    selection[0] = 23;
    correct[0] = false;
    score[0] = 12920;
    Console.WriteLine($"Welcome to Learning about Hardware {selection[0]}");
    Console.WriteLine($"Your score is {score[0]}");
    Console.WriteLine($"Correct: {correct[0]}");
}

Welcome();
```

## 
```c#
string question = "What three things do electronic hardware devices need in order to function?";

string[] answers = new string[3];

void PrintAll()
{
    Console.WriteLine(question);
    Console.WriteLine("1. Power supply, CPU, Software.");
    Console.WriteLine("2. TV, Hardware, Cellphone or Battery.");
    Console.WriteLine("3. CPU, Software, Mouse and Keyboard.");
    
    answers[0] = "Power supply, CPU, Software.".ToLower();
    answers[1] = "TV, Hardware, Cellphone or Battery.";
    answers[2] = "CPU, Software, Mouse and Keyboard.";

    Console.WriteLine(answers[0]);
}

PrintAll();
```


```c#
string[] answers = { "Power supply, CPU, Software.", "TV, Hardware, Cellphone or Battery.", "CPU, Software, Mouse and Keyboard." };
void loopThrough()
{
    foreach (string an in answers)
    {
        if (an == "Power supply, CPU, Software.")
        {
            Console.WriteLine("Correct answer: " + an.Split(", , ,")[0]);
        }
        else
        {
            Console.WriteLine("Incorrect answer: " + an.Split(", , ,")[0]);
        }
    }
}
loopThrough();
```


# Best Practice 
```c#
void ShowData(string a, int b, int c);
void DisplayDate(string month, int day, int year);

ShowData("Hello", 5, 10);
DisplayDate("January", 1, 2022);
```

# 
```c#
void ShowData(string a, int b, int c);
void DisplayDate(string month, int day, int year);
```


```c#
void ShowData(string a, int b, int c){
    Console.WriteLine(a);
    Console.WriteLine(b);
    Console.WriteLine(c);
}
void DisplayDate(string month, int day, int year){
    Console.WriteLine(month);
    Console.WriteLine(day);
    Console.WriteLine(year);
}

ShowData("Hello", 5, 10);
DisplayDate("January", 1, 2022);
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