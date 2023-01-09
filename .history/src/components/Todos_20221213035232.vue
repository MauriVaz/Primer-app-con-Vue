<template>
    <div class="container">
        <div v-bind:key="todo.id" v-for="todo in todoslist">
            <TodoItem>
        </div>
    </div>
</template>

<script>
import TodoItem from './TodoItem.vue';

export default{
    // eslint-disable-next-line vue/multi-word-component-names
    name: "Todos",
    props: ["todoslist"],
    components: { TodoItem }
}
</script>

<style>
.container{
    background-color: lightgreen;
    padding:4vh;
}
</style>
