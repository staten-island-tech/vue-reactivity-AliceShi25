<template>
  <div class="YourCart">
    <img :src="img" alt="" class="img2" />
    <h3>{{ lastname }} {{ name }}</h3>
    <button @click="remove(item)">Annul Investment</button>
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
    img: String,
  },
  methods: {
    remove(item) {
      this.store.cart = this.store.cart.filter((t) => t !== item);
      console.log(item);
    },
  },
};
</script>

<style scoped>
.YourCart {
  margin: 0.5rem;
}

.img2 {
  width: 50%;
  border-radius: 1.5rem;
}
</style>
