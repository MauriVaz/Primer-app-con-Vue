<template>
    <div class="container">
        <div v-bind:key="todo.id" v-for="todo in todoslist">
            <TodoItem v-bind:todo="todo"/>
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
    background-color: gray;
    padding:4vh;
}
</style>
