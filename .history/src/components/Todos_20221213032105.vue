<template>
    <div>
        <div v-for="todo in todoslist">
<div>{{Todo.title}}</div>
        </div>
    </div>
</template>

<script>
export default{
    name:"Todos",
    props:['todoslist']
}
</script>

<style>
</style>
