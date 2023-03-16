<template>
  <div class="hewwo">
    <h1>hello</h1>
    <h2 v-if="notcat">{{ weewo }}</h2>
    <h2 v-else>Yai9dosskjhksa</h2>
    <ul>
      <li v-for="cat in cats" :key="cat">{{ cat }}</li>
    </ul>
    <div class="button">
      <button v-on:click="yessir" v-if="mewozzy">Mewozaaa!</button>
      <button v-on:click="yessir" v-else>wroof</button>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      weewo: "mewo",
      cats: ["cat1", "mewmewo", "bbg", "kitty", "somewo"],
      notcat: true,
      mewozzy: true,
    };
  },
  methods: {
    yessir: function () {
      if (this.mewozzy === false) {
        this.mewozzy = true;
      } else {
        this.mewozzy = false;
      }
    },
  },
};
</script>

<style scoped>
.hewwo {
  color: pink;
  text-align: center;
}
</style>
