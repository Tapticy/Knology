# Short while loop
```c#
    int secret = 5;
    int guess;
    Console.WriteLine("Secret number is between 1 - 10");

    do {
        guess = 7;
        Console.WriteLine($"Number is : {guess}");

        if (guess < secret) {
            Console.WriteLine("Too Low");
        }
        else if (guess > secret) {
            Console.WriteLine("Too high");
        }

    } while (guess != secret);
    Console.WriteLine("Correct Number");
```

# A to do while loop
```c#
 int guess = 0, youNumber;
 string hint;

 int secretNumber = (new Random()).Next(1, 10);
 Console.WriteLine("1 Between 10");

do {
    guess++;
    Console.Write($"Turns: {guess}");
    youNumber = Convert.ToInt32(Console.ReadLine());

    if (youNumber < secretNumber) {
        hint = $"Your guess: {youNumber} is low";
    }
    else if (youNumber > secretNumber) {
        hint = $"Your guess: {youNumber} is high";
    }
    else {
        hint = $"Bingo Nice guess {guess}";
    }
    Console.WriteLine(hint);

} while (guess < 4 && youNumber != secretNumber);

if (youNumber != secretNumber) {
    Console.WriteLine("Ooops you lost");
}
```

# Small while loop 
```c#
int count = 1;

do {
    Console.WriteLine("Value: {0}", count);
    count = count + 1;

} while (count < 20);
Console.ReadLine();
```



```c#
double number = 0, total = 0, count = 0, average = 0;

string input = "";

Console.WriteLine("Enter A list number type Q to exit");

while (input != "Q" && input != "q") {
    input = Console.ReadLine();
    if (input != "Q" && input != "q") {
        number = Convert.ToDouble(input);
        total += number;
        count++;
    }
}

if (count > 0) {
    average = total / count;
}

Console.WriteLine($"Average: {average}");
```