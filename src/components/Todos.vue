<template>
  <div>
    <div v-bind:key="todo.id" v-for="todo in todos_x">
      <TodoItem v-bind:todo="todo"/>
    </div>
  </div>
</template>

<script>
import TodoItem from "./TodoItem.vue";

export default {
  name: "Todos",
  components: {
    TodoItem
  },
  props: ["todos_x"]
};
</script>