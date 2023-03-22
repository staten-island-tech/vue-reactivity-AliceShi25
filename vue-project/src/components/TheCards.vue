<template>
  <div class="stuffs">
    <div class="stuff">
      <h2>{{ lastname }} {{ name }}</h2>
      <img :src="image" alt="" class="img" />
    </div>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: {
    lastname: String,
    name: String,
    image: String,
  },
};
</script>

<style scoped>
/* .cards {
  flex: 0 0 23.5%;
  width: 32vw;
  margin-bottom: 10rem;
  background-color: pink;
  align-content: center;
  border: solid white;
  border-radius: 25px;
} */
</style>
