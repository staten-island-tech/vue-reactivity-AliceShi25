<template>
  <div class="cards">
    <img :src="img" alt="" class="img" />
    <h3>{{ lastname }} {{ name }} ({{ group }})</h3>
    <button @click="push()" class="btn">Invest!!!</button>
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
    price: Number,
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
      store.total += this.price;
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

.btn {
  font-family: "Alkatra", cursive;
  display: inline-block;
  color: white;
  cursor: pointer;
  background-color: #1b1545;
  font-size: 1rem;
  text-align: center;
  border-radius: 5rem;
  width: 15vw;
  transition: all 0.3s;
  position: relative;
}

.btn:hover {
  box-shadow: 0 1.5px 5px pink;
  color: grey;
  background-color: #f4fdff;
  border: solid pink;
}

.img {
  width: 100%;
  border-radius: 1.5rem;
  box-shadow: 0.2px 4px 5px grey;
}
</style>
