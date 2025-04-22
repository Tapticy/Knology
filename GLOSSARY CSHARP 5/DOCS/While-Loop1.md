```c#
string? user;
bool valid = false;

Console.WriteLine("Enter Below");
do
{
    user = Console.ReadLine();
    if (user != null)
    {
        if (user.Length >= 5)
        {
            valid = true;
            Console.WriteLine($"{valid} You have {user} letter");
        }
        else
        {
            Console.WriteLine("Your Input Invalid");
        }
    }
} while (valid == false);
```