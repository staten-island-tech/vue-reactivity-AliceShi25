<template>
  <div class="cards">
    <img :src="img" alt="" class="img" />
    <h3>{{ lastname }} {{ name }} ({{ group }})</h3>
    <button @click="push()">Invest!!!</button>
  </div>
</template>

<script>
import { store } from "./store";
// import TheButton from "../components/TheButton.vue";
export default {
  name: "Card",
  components: {},
  props: {
    lastname: String,
    name: String,
    img: String,
    group: String,
  },
  data() {
    return {
      store,
    };
  },
  methods: {
    push() {
      store.cart.push({
        lastname: this.lastname,
        name: this.name,
        img: this.img,
      });
    },
  },
};
</script>

<style scoped>
.cards {
  width: 15rem;
  margin: 0.5rem;
  color: white;
}

.img {
  width: 100%;
  border-radius: 1.5rem;
  box-shadow: 0.2px 4px 5px grey;
}
</style>
