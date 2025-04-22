
# Input and Button
```c#
<input />
<button>Add todo</button>

<ul>
    @foreach (var todo in todos)
    {
        <li>@todo.Title</li>
    }
</ul>


@code {
    private List<TodoItem> todos = new();
    string newTodo = "";
}
```

