<template>
  <div class="YourCart">
    <h3>{{ lastname }} {{ name }}</h3>
    <button>Annul Investment</button>
  </div>
</template>

<script>
import { store } from "./store";
export default {
  name: "Cart",
  data() {
    return { store };
  },
  props: {
    lastname: String,
    name: String,
    image: String,
  },
};
</script>

<style scoped>
.YourCart {
  color: black;
  background-color: white;
  width: 10%;
}
</style>
