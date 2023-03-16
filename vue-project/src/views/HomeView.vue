<template>
  <div class="hewwo">
    <h1>hello</h1>
    <h2 v-if="notcat">{{ weewo }}</h2>
    <h2 v-else>Yai9dosskjhksa</h2>
    <ul>
      <li v-for="item in items" :key="item.name">{{ item.name }}</li>
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
      items: [
        { name: "Tyler", lastName: "Bo", osis: "2048n6125" },
        { name: "A", lastName: "S", osis: "nnnnnnnnn" },
        { name: "AB", lastName: "ST", osis: "nnnnwnnnn" },
      ],
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
