<template>
  <div class="cards">
    <img :src="image" alt="" class="img" />
    <h2>{{ lastname }} {{ name }} ({{ group }})</h2>
    <button>Invest!!!</button>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: {
    lastname: String,
    name: String,
    image: String,
    group: String,
  },
};
</script>

<style scoped>
.cards {
  width: 300px;
  margin: 1rem;
  border-radius: 3px;
  box-shadow: 0.2px 4px 5px black;
  background-color: lightgray;
}

.img {
  width: 100%;
}
</style>
