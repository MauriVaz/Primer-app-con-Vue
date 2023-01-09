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
  },data(){
    return{
      todos:[
        {
          id:0,
          title:"Comprar la cena",
          completed:false
        }
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
