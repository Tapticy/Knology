# Working on
```c#
        #region
        #endregion
```

# 
```c#
char[] letters = { 'f', 'r', 'e', 'd', ' ', 's', 'm', 'i', 't', 'h' };
        string name = "";
        int[] a = new int[10];
        for (int i = 0; i < letters.Length; i++) {
            name += letters[i];
            a[i] = i + 1;
            SendMessage(name, a[i]);
        }
        Console.ReadKey();

        static void SendMessage(string name, int msg) {
            Console.WriteLine($"Hi {name} I Count to {msg}");
        }
```

