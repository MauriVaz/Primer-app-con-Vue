<template>
    <div id="add-container" >
        <form @submit="addTodo">
            <input type="text" v-model="title" />
        </form>
    </div>
</template>

<script>

export default {
    name:'TodoAdd',
    data(){
        return  {
            title:""
        }
    },
    methods:{
        addTodo(e){
            e.preventDefault()
        }
    }
}
</script>

<style scoped>
    #add-container{
        padding: 10px;
    }
    input{
        padding:10px;
        outline:none;
        border:solid 1px #ccc;
        width:100%;
    }
</style>
