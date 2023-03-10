<script>
import { Ref } from "vue";
let id = 0;
export default {
  data() {
    return {
      message: "mewmew",
      sameww: "meow",
      count: 0,
      text: "",
      lyuvee: true,
      newTodo: "",
      todos: [
        { id: id++, text: "Learn HTML" },
        { id: id++, text: "Learn JavaScript" },
        { id: id++, text: "Learn Vue" },
      ],
    };
  },
  methods: {
    littlemew() {
      // update component state
      this.count++;
    },
    onInput(e) {
      this.text = e.target.value;
    },
    toggle() {
      this.lyuvee = !this.lyuvee;
    },
    addTodo() {
      this.todos.push({ id: id++, text: this.newTodo });
      this.newTodo = "";
    },
    removeTodo(todo) {
      this.todos = this.todos.filter((t) => t !== todo);
    },
  },
};
</script>

<template>
  <h1 v-bind:class="sameww">{{ message }}</h1>
  <button @click="littlemew">{{ count }}</button>
  <button @click="toggle">
    <h1 v-if="lyuvee">heweeoewo</h1>
    <h1 v-else>hehiajak</h1>
  </button>
  <input :value="text" @input="onInput" placeholder="Type here" />
  <p>{{ text }}</p>
  <form @submit.prevent="addTodo">
    <input v-model="newTodo" />
    <button>Add Todo</button>
  </form>
  <ul>
    <li v-for="todo in todos" :key="todo.id">
      {{ todo.text }}
      <button @click="removeTodo(todo)">X</button>
    </li>
  </ul>
</template>

<style scoped>
.meow {
  color: aqua;
}
</style>
