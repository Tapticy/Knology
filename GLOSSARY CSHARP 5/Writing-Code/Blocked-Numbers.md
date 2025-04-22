# Block Numbers 
Need to block or ???

1 506-451-5856
1 807-444-7146
1 519-851-7875
1 306-514-2135

1 367-890-0161
1 514-805-3213
1 418-265-3382

1 437-564-1032
1 647-873-3657
1 782-612-0095
1 289-802-8634
1 581-893-7340
1 647-600-1148

1 579-984-5166
1 639-812-4710
1 438-619-7431

```c#
string[] one = ["438-619-7431", "639-812-4710", "514-805-3213","367-890-0161", "519-851-7875", "306-514-2135", "807-444-7146", "506-451-5856"];

string[] two = ["579-984-5166", "647-600-1148", "581-893-7340", "289-802-8634", "782-612-0095", "647-873-3657", "437-564-1032", "418-265-3382"];
```

# Just Example working on
```c#
string[] one = ["438-619-7431", "639-812-4710", "514-805-3213","367-890-0161", "519-851-7875", "306-514-2135", "807-444-7146", "506-451-5856"];

string[] two = ["579-984-5166", "647-600-1148", "581-893-7340", "289-802-8634", "782-612-0095", "647-873-3657", "437-564-1032", "418-265-3382"];


Console.WriteLine("Blocked Numbers \n");
foreach (string n in one){
    
    Console.WriteLine($"{n}"); 
}

```

6245

1 418-474-9756
1 519-557-0545
1 519-552-2780
1 647-600-1153
1 226-234-6645


```c#

string[] blockedOne = ["438-619-7431", "639-812-4710", "514-805-3213","367-890-0161", "519-851-7875", "306-514-2135", "807-444-7146", "506-451-5856"];

string[] blockedTwo = ["579-984-5166", "647-600-1148", "581-893-7340", "289-802-8634", "782-612-0095", "647-873-3657", "437-564-1032", "418-265-3382"];

string[] blockedThree = ["4184749756", "519-557-0545", "519-552-2780",
 "647-600-1153", "226-234-6645"];

string checkNumber = Console.ReadLine();
string checkNewNumber = checkNumber.Replace("-", "");


Console.Beep();

if (checkNumber == checkNewNumber){
    Console.WriteLine("Please enter your phone that you are calling from");
    checkNumber = Console.ReadLine();
    Console.WriteLine("Please leave a message after the tone " + checkNumber);
}

if (blockedOne.Contains(checkNumber))
{
    Console.WriteLine("Blocked");
}
else if (blockedTwo.Contains(checkNumber))
{
    Console.WriteLine("Blocked");
}
else if (blockedThree.Contains(checkNumber))
{
    Console.WriteLine("Blocked");
}
else
{
    Console.WriteLine("Not blocked");
}
```