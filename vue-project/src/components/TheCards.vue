<template>
  <div class="cards">
    <img :src="image" alt="" class="img" />
    <h3>{{ lastname }} {{ name }} ({{ group }})</h3>
    <button>HELP</button>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  name: "Card",
  props: {
    lastname: String,
    name: String,
    image: String,
    group: String,
  },
  methods: {},
};
</script>

<style scoped>
.cards {
  width: 300px;
  margin: 1rem;
  color: white;
}

.img {
  width: 100%;
  border-radius: 1.5rem;
  box-shadow: 0.2px 4px 5px grey;
}
</style>
