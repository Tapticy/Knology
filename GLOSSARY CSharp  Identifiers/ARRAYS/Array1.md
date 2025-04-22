
# Using For Loop  For() Method
```c#
int currentAssignment = 0;
int sophiaSum = 0;
int andrewSum = 0;
int emmaSum = 0;
int loganSum = 0;

int[] sophiaScores = new int[] { 90, 86, 87, 98, 100 };

int[] andrewScores = new int[] { 92, 89, 81, 96, 90 };

int[] emmaScores = new int[] { 90, 85, 87, 98, 68 };

int[] loganScores = new int[] { 90, 95, 87, 88, 96 };

for (currentAssignment = 0; currentAssignment < sophiaScores.Length; currentAssignment++)
{
    sophiaSum += sophiaScores[currentAssignment];
    andrewSum += andrewScores[currentAssignment];
    emmaSum += emmaScores[currentAssignment];
    loganSum += loganScores[currentAssignment];
    Console.WriteLine($"Current Assignment: {currentAssignment}");
    Console.WriteLine($"Sophia's Sum: {sophiaSum}");
    Console.WriteLine($"Andrew's Sum: {andrewSum}");
    Console.WriteLine($"Emma's Sum: {emmaSum}");
    Console.WriteLine($"Logan's Sum: {loganSum}");
}
```


# Example 2
```c#
// initialize variables - graded assignments 
int currentAssignments = 5;

// Student names
string[] studentNames = new string[] { "Sophia", "Andrew", "Emma", "Logan" };

int[] sophiaScores = new int[] { 90, 86, 87, 98, 100 };
int[] andrewScores = new int[] { 92, 89, 81, 96, 90 };
int[] emmaScores = new int[] { 90, 85, 87, 98, 68 };
int[] loganScores = new int[] { 90, 95, 87, 88, 96 };


foreach (string name in studentNames)
{
    
    if (name == "Emma"){
           int sophiaSum = 0;
           decimal sophiaScore;
           
           foreach (int score in sophiaScores){
           // Sum of all scores
           sophiaSum += score;
           }
        sophiaScore = (decimal)sophiaSum / currentAssignments;
        
        Console.WriteLine("Student\t\tGrade\n");
        Console.WriteLine("Sophia:\t\t" + sophiaScore + "\tA-");
    }

}
Console.WriteLine("Press the Enter key to continue");
Console.ReadLine();
```

# Example 3
```c#
// initialize variables - graded assignments 
int currentAssignments = 5;

// Student names
string[] studentNames = new string[] { "Sophia", "Andrew", "Emma", "Logan" };

int[] sophiaScores = new int[] { 90, 86, 87, 98, 100 };
int[] andrewScores = new int[] { 92, 89, 81, 96, 90 };
int[] emmaScores = new int[] { 90, 85, 87, 98, 68 };
int[] loganScores = new int[] { 90, 95, 87, 88, 96 };

int[] studentScores = new int[10];

foreach (string name in studentNames)
{
    string currentStudent = name;
    
    if (name == "Emma"){
           int sophiaSum = 0;
           decimal sophiaScore;
           
           foreach (int score in sophiaScores){
           // Sum of all scores
           sophiaSum += score;
           }
        sophiaScore = (decimal)sophiaSum / currentAssignments;
        
        Console.WriteLine("Student\t\tGrade\n");
        Console.WriteLine("Sophia:\t\t" + sophiaScore + "\tA-");
    }

}

Console.WriteLine("Press the Enter key to continue");
Console.ReadLine();
```



# Example 4
```c#
// initialize variables - graded assignments 
int currentAssignments = 5;

// Student names
string[] studentNames = new string[] { "Sophia", "Andrew", "Emma", "Logan" };

int[] sophiaScores = new int[] { 90, 86, 87, 98, 100 };
int[] andrewScores = new int[] { 92, 89, 81, 96, 90 };
int[] emmaScores = new int[] { 90, 85, 87, 98, 68 };
int[] loganScores = new int[] { 90, 95, 87, 88, 96 };

int[] studentScores = new int[10];



foreach (string name in studentNames)
{
    string currentStudent = name;
    
    if (currentStudent == "Sophia")
        studentScores = sophiaScores;

    else if (currentStudent == "Andrew")
        studentScores = andrewScores;

    else if (currentStudent == "Emma")
        studentScores = emmaScores;

    else if (currentStudent == "Logan")
        studentScores = loganScores;
    

    int sophiaSum = 0;
    decimal sophiaScore;
           
    foreach (int score in sophiaScores){
    // Sum of all scores
    sophiaSum += score;
    }
    
    sophiaScore = (decimal)sophiaSum / currentAssignments;
        
    Console.WriteLine("Student\t\tGrade\n");
    Console.WriteLine("Sophia:\t\t" + sophiaScore + "\tA-");

}


Console.WriteLine("Press the Enter key to continue");
Console.ReadLine();

```


# Example 
```c#


```