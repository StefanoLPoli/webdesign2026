<script>
    let todos = $state([
        { title: "Assignment 1", done: true },
        { title: "Assignment 2", done: false },
        { title: "Assignment 3", done: false }
    ]);
</script>

<h3>My Todo List</h3>

<ul>
    {#each todos as todo}
        <li>
            <input type="checkbox" bind:checked={todo.done}>
            <span class:done={todo.done}>{todo.title}</span>
        </li>
    {/each}
</ul>