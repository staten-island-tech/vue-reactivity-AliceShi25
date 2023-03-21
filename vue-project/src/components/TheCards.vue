<template>
  <div class="card">
    <div class="cards">
      <h2>{{ lastname }} {{ name }}</h2>
      <img src="" alt="" />
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

.cards {
  flex: 0 0 23.5%;
  width: 32vw;
  margin: 25px auto;
  background-color: red;
  align-content: center;
  border: solid white;
  border-radius: 25px;
}

.card {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  flex-direction: row;
  padding: 2.5rem;
  text-align: center;
}
</style>
