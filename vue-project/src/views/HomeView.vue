<template>
  <div class="hewwo">
    <h1>hello</h1>
    <h2>{{ weewo }}</h2>
    <ul>
      <li v-for="cat in cats" :key="cat">{{ cat }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      weewo: "mewo",
      cats: ["cat1", "mewmewo", "bbg", "kitty", "somewo"],
    };
  },
};
</script>

<style scoped>
.hewwo {
  color: pink;
  text-align: center;
}
</style>
