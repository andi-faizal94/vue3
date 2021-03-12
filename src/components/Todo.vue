<template>
  <div>
    <h3>Todolist</h3>

    <h6 v-for="(todo, index) in todos" :key="index">{{todo}}</h6>
    <p>{{todos.task}}</p>
    <input v-model="todos.task" placeholder="text" />
    <input type="button" value="button" />
  </div>
</template>

<script>
export default {
  name: "Todo",
  data() {
    return {
      todos: [
        {
          id: 1,
          task: ""
        }
      ]
    };
  }
};
</script>

<style scoped>
</style>