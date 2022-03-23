<template>
  <div class="app">
    <h1>Todo application</h1>
    <hr>
    <TodoList
      v-bind:todos="todos"
    />
  </div>
</template>

<script>
import TodoList from './TodoList'
export default {
  name: 'App',
  data () {
    return {
      todos: [
        {id: 1, title: 'Купить лекарства', completed: false},
        {id: 1, title: 'Купить хлеб', completed: false},
        {id: 1, title: 'Купить масло', completed: false}
      ]
    }
  },
  components: {
    TodoList
  }
}
</script>

<style  lang="scss">
.app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
