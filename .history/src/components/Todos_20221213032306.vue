<template>
    <div>
        <div v-bind:key="todo.id" v-for="todo in todoslist">
            <div>{{Todo.title}}</div>
        </div>
    </div>
</template>

<script>
export default{
    // eslint-disable-next-line vue/multi-word-component-names
    name:'Todos',
    props:['todoslist']
}
</script>

<style>
</style>
