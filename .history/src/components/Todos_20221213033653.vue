<template>
    <div class="container">
        <div v-bind:key="todo.id" v-for="todo in todoslist">
            <div>{{todo.title}}</div>
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
.container{
    background-color: lightgreen;
}
</style>
