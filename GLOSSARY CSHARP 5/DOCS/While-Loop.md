# The Difference Between Do and While statement iterations
# While Loop
i++ increment i-- decrement
here Initialized variable that iterates with `int i = draw1.Length`.
```c#
Random ran = new Random();
int current = ran.Next(01, 50);

/*
do
{
    current = ran.Next(1, 15);
    Console.WriteLine(current);
} while (current == 5);
*/

while (current >= 10)
{
    Console.WriteLine(current);
    current = ran.Next(1, 20);
}
Console.WriteLine($"Last Number: {current}");
```


# The Difference Between Do and While statement iterations?
## string?


This code below will still run but will return an error: 
`The annotation for nullable reference types should only be used in code within a '#nullable' annotations context`

To fix this all you have to do is use the `#nullable enable` 
```c#
string? readResult;
Console.WriteLine("Enter a string:");
do
{
    readResult = Console.ReadLine();
} while (readResult == null);
    Console.WriteLine(readResult);
```


# If Statement Inside Of A Do While 
## continue 
```c#
int hero = 10;
int monster = 10;
Random ice = new Random();

do
{
    int rolling = ice.Next(1, 11);
    monster -= rolling;
    Console.WriteLine($"Monster Lost\n {rolling} of health");

    if (monster <= 0)
        continue;

    rolling = ice.Next(1, 11);
    hero -= rolling;
    Console.WriteLine($"Hero Lost\n {rolling} has now {hero}");
} while (hero > 0 && monster > 0);

Console.WriteLine(hero > monster ? "Hero Wins" : "Monster Wins");
```

# Project 1
The code uses a do statement because the code block must be executed at least once. You CAN also use a while to achieve the same result. Some developers may feel that the logic of a while makes the code more readable. If that's the case for you, you can choose to implement a while statement here.
```c#
string? readResult;
string valueEntered = "";
int numValue = 0;
bool validNumber = false;

Console.WriteLine("Enter an integer value between 5 and 10");

do
{
    readResult = Console.ReadLine();
    if (readResult != null) 
    {
        valueEntered = readResult;
    }

    validNumber = int.TryParse(valueEntered, out numValue);

    if (validNumber == true)
    {
        if (numValue <= 5 || numValue >= 10)
        {
            validNumber = false;
            Console.WriteLine($"You entered {numValue}. Please enter a number between 5 and 10.");
        }
    }
    else 
    {
        Console.WriteLine("Sorry, you entered an invalid number, please try again");
    }
} while (validNumber == false);

Console.WriteLine($"Your input value ({numValue}) has been accepted.");

readResult = Console.ReadLine();
```

# Project 2
The following code is one possible solution for challenge project 2 from the previous unit.

The code uses a do statement because the code block must be executed at least once. You CAN also use a while to achieve the same result. Some developers may feel that the logic of a while makes the code more readable. If that's the case for you, you can choose to implement a while statement here.
```c#
string? readResult;
string roleName = "";
bool validEntry = false;

do
{
    Console.WriteLine("Enter your role name (Administrator, Manager, or User)");
    readResult = Console.ReadLine();
    if (readResult != null)
    {
        roleName = readResult.Trim();
    }

    if (roleName.ToLower() == "administrator" || roleName.ToLower() == "manager"
        || roleName.ToLower() == "user")
    {
        validEntry = true;
    }
    else
    {
        Console.Write($"The role name that you entered, \"{roleName}\" is not valid. ");
    }
} while (validEntry == false);

Console.WriteLine($"Your input value ({roleName}) has been accepted.");
readResult = Console.ReadLine();
```


# Project 3
The following code is one possible solution for challenge project 3 from the previous unit.

The code uses a for statement for the outer loop because you cannot modify the value assigned to a 'foreach iteration variable'. You could work around this by declaring an extra string variable inside the foreach loop, but then you would be adding unwanted complexity to your code logic. In other words, using the iteration statement foreach (string myString in myStrings) and then attempting to process the myString variable generates a compilation error.

The code uses a while statement for the inner loop because, depending on the value of the data string, the code block may not be executed (when the string does not contain a period). You should not use a do statement in situations where the iteration block may not need to be executed
```c#
string[] myStrings = new string[2] { "I like pizza. I like roast chicken. I like salad", "I like all three of the menu choices" };
int stringsCount = myStrings.Length;

string myString = "";
int periodLocation = 0;

for (int i = 0; i < stringsCount; i++)
{
    myString = myStrings[i];
    periodLocation = myString.IndexOf(".");

    string mySentence;

    // extract sentences from each string and display them one at a time
    while (periodLocation != -1)
    {

        // first sentence is the string value to the left of the period location
        mySentence = myString.Remove(periodLocation);

        // the remainder of myString is the string value to the right of the location
        myString = myString.Substring(periodLocation + 1);

        // remove any leading white-space from myString
        myString = myString.TrimStart();

        // update the comma location and increment the counter
        periodLocation = myString.IndexOf(".");

        Console.WriteLine(mySentence);
    }
 
    mySentence = myString.Trim();
    Console.WriteLine(mySentence);
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