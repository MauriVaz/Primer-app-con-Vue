<template>
    <div>
        <h1>Lista de todos</h1>
        <div v-bind:key="todo.id" v-for="todo in todoslist">
            <TodoItem v-bind:todo="todo" v-on:delete-todo="$emit('delete-todo', todo.id)" />
        </div>
    </div>
</template>

<script>
import TodoItem from './TodoItem';

    export default {
        // eslint-disable-next-line vue/multi-word-component-names
        name: 'Todos',
        props: ['todoslist'],
        components:{TodoItem}
    }
</script>

<style></style>