
# 
```c#
@page "/counter"


<PageTitle>Counter</PageTitle>

<h1>Counter</h1>

<p role="status">Current count: @currentCount</p>

<button class="btn btn-primary" @onclick="IncrementCount">Click me</button>


@code {
    private int currentCount = 0;
      
    private void IncrementCount()
    {
        currentCount++;
    }
}


<br> <br> <br>
<input @onchange="InputChanged" />
<p>@message</p>

@code {
    string message = "";

    void InputChanged(ChangeEventArgs e)
    {
        message = (string)e.Value;
    }
}
```


# Data Blinding
### Button Event Change
```c#
<input @bind="text" />
<button @onclick="() => text = string.Empty">Clear</button>
<br> <br>


@code {
    string text = "";
}
```