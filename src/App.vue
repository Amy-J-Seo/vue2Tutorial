<template>
  <div id="app">
  <h1>hello</h1>
  <Todos v-bind:todos="todos"/>
  </div>
</template>

<script>
import Todos from './components/Todos.vue';

export default {
  name: 'App',
  components: {
    Todos
    
  },
  data(){
    return{
      todos:[
        {
          id:1,
          title: "one",
          completed:false
        },
        {
          id:2,
          title: "two",
          completed:true
        },
        {
          id:3,
          title: "three",
          completed:false
        },
        ]
    }
    }
}
</script>

<style>
*{
  box-sizing: border-box;
  margin:0;
  padding:0;
  }

  body{
    font-family: Arial, Helvetica, sans-serif;
    line-height: 1.4;
    }
</style>
