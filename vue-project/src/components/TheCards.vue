<template>
  <div class="cards">
    <img :src="image" alt="" class="img" />
    <h3>{{ lastname }} {{ name }} ({{ group }})</h3>
    <button v-on:click="push()">HELP</button>
  </div>
</template>

<script>
import { invest } from "./invest.js";
export default {
  data() {
    return {
      invest,
    };
  },
  name: "Card",
  props: {
    lastname: String,
    name: String,
    image: String,
    group: String,
  },
  methods: {
    push() {
      this.invest.cart.push({ lastname: this.lastname, name: this.name });
    },
  },
};
</script>

<style scoped>
.cards {
  width: 20rem;
  margin: 0.5rem;
  color: white;
}

.img {
  width: 100%;
  border-radius: 1.5rem;
  box-shadow: 0.2px 4px 5px grey;
}
</style>
