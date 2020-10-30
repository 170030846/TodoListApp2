<template>
  <div id="app" class="container">
    <div class="todolist">
 <img alt="Vue logo" src="./assets/logo.png" class="logo">
    <h3 style="text-align: center">Todo APP</h3>
   <TodoList/>
    </div>
   

  </div>
</template>

<script>

import TodoList from './components/TodoList'

export default {
  name: 'App',
  components: {
    TodoList
  }
}
</script>

<style>

*{
  box-sizing: border-box;
  
}
html{
  background:#90f1c6;
  overflow-y: scroll;
  overflow-x: hidden;
  height: 100%;
}


.container{
  max-width: 600px;
  margin: 0 auto;
  
}
.todolist{
   min-height: 50vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  border-radius: 1em;
  background: #fff;
  overflow: hidden;
  box-shadow: 0 0 5px rgba(25,25,25,.25);
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  font-size: 24px;
}

.logo{
  display: block;
  margin: 20px auto;
  height: 75px;
}
</style>
