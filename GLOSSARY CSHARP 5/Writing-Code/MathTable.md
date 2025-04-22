
# Multiplication Tables
```c#
public class Exercise7 // Declaration of the Exercise7 class
{
    public static void Main() // Main method, entry point of the program
    {
        int j,
            i,
            n; // Declaration of variables 'j' and 'i' for iteration and 'n' to store the input number

        Console.Write("\n\n"); // Displaying new lines
        Console.Write("Display the multiplication table vertically from 1 to n:\n"); // Displaying the purpose of the program
        Console.Write("---------------------------------------------------------"); // Displaying a separator
        Console.Write("\n\n");

        Console.Write("Input up to the table number starting from 1 : "); // Prompting the user to input a number for the multiplication table
        n = Convert.ToInt32(Console.ReadLine()); // Reading the number entered by the user

        Console.Write("Multiplication table from 1 to {0} \n", n); // Displaying the range of multiplication table

        for (i = 1; i <= 10; i++) // Outer loop to generate rows for the multiplication table up to 10
        {
            for (j = 1; j <= n; j++) // Inner loop to generate columns for each number up to 'n'
            {
                if (j <= n - 1) // Checking if it's not the last column of the table
                    Console.Write("{0}x{1} = {2}, ", j, i, i * j); // Displaying the multiplication table entry with comma separation
                else
                    Console.Write("{0}x{1} = {2}", j, i, i * j); // Displaying the multiplication table entry for the last column
            }
            Console.Write("\n"); // Moving to the next line after completing a row in the table
        }
    }
}

```