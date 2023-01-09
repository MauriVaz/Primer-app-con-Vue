<template>
    <div>
        <div class="todo-body">
            <input type="checkbox" />
            {{todo.title}}
        </div>
        <div class="todo-actions">
            <button>Eliminar</button>
        </div>
    </div>
</template>

<script>
export default{
    name:"TodoItem",
    props:['todo']
}
</script>

<style scoped>
.todo{
    border-bottom:solid 1px #ccc
}
</style>
