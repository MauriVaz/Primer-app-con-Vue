<template>
    <div id="add-container">
        <form @submit="addTodo">
            <input type="text" placeholder="Añadir todo" v-model="title">
            <label for="cars">Choose a car:</label>

<select id="cars">
  <option label="Volvo">Volvo (Latin for "I roll")</option>
  <option label="Saab">Saab (Swedish Aeroplane AB)</option>
  <option label="Mercedes">Mercedes (Mercedes-Benz)</option>
  <option label="Audi">Audi (Auto Union Deutschland Ingolstadt)</option>
</select>
        </form>
    </div>
</template>

<script>
import { uuid } from 'vue-uuid';

export default {
    name: 'TodoAdd',
    data(){
        return {
            title: ''
        }
    },
    methods:{
        addTodo(e){
            e.preventDefault();

            const newTodo = {
                id: uuid.v4(),
                title: this.title.charAt(0).toLocaleUpperCase() 
                + this.title.toLocaleLowerCase().substring(1, this.title.length),
                completed: false
            };

            this.title = '';
            this.$emit('add-todo', newTodo);
        }
    }
}
</script>

<style scoped>
    #add-container{
        padding: 10px;
    }
    input{
        padding: 10px;
        outline: none;
        border: solid 1px #ccc;
        width: 100%;
    }
</style>