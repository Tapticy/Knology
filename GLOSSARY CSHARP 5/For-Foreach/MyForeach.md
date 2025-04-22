
# Wrong need to look at
The `question` is missing `; expected` and the end of the 
assigned string `string question = "How many bits are in a byte?";`.

The if statement as a type string and int that cannot be applied, because 
any of the types string or integers has be converted or loop through a for loop is a better practice. 
```c#
string question = "How many bits are in a byte?"
int[] answers = [8, 4, 7]; 
Console.WriteLine(question);
Console.WriteLine("");
string userAnswer = Console.ReadLine();

if (userAnswer == answers[1]){
    Console.WriteLine("Correct!");
}
else if (userAnswer == answers[0]){
    Console.WriteLine("Not 4 Bits Sorry!");
}
else if (userAnswer == answers[2]){
    Console.WriteLine("Not 7 Bits Sorry!");
}
else {
    Console.WriteLine("Try Again!");
}
```

# Better Practice
```c#
  string question = "How many bits are in a byte?";
  int[] answers = [8, 4, 7];
  Console.WriteLine(question);
  Console.WriteLine("");
  string? userAnswer = Console.ReadLine();
  for (int i = 0; i < answers.Length; ++i) {
      if (answers[i] == 7) {
          foreach (int e in answers) {
              Console.WriteLine($"{e}");
          }
      }
      else {
          Console.WriteLine("Try Again");
      }
  }
```
