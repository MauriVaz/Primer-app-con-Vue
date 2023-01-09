<template>
  <div id="header"></div>
  <div id="main-container">
    <h2>Todos</h2>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Search from './components/Search.vue';
import Todos from './components/Todos.vue';
import TodoApp from "./components/TodoApp.vue"
export default {
  name: 'App',
  components: {
    Search,Todos,TodoApp
  },
  data(){
    return{
      todos:[
        {
          id:0,
          title:"Comprar la cena",
          completed:false
        },{
          id:1,
          title:"Sacar a pasear al perro",
          completed:true
        },{
          id:2,
          title:"Jugar XBOX",
          completed:false
        }
      ],
      copyTodos:[]
    }
  },
  created(){
    this.copyTodos=[...this.todos]
  }
}
</script>

<style>
*{box-sizing: border-box;}

body{
  font-family: Arial, Helvetica, sans-serif;
  font-size: 1.5em;
  padding: 0;
  margin: 0;
 }
 #main-container{
   border: solid 1px  #ccc;
   width: 600px;
   margin: 100px auto;}
 

</style>
