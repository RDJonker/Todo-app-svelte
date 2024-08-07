<script lang="ts">
    type clearCompletedType = () => void
    type CompletedTodos = number

    export let clearCompleted: clearCompletedType
    export let completedTodos: CompletedTodos
</script>

<button 
on:click={clearCompleted}
    class:hidden={completedTodos === 0}
    class="clear-completed"
    >
    Clear completed
</button>