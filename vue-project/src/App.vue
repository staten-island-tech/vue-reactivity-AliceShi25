<script>
export default {
  data() {
    return {
      message: "mewmew",
      sameww: "meow",
      count: 0,
    };
  },
  methods: {
    littlemew() {
      // update component state
      this.count++;
    },
  },
};
</script>

<template>
  <h1 v-bind:class="sameww">{{ message }}</h1>
  <button @click="littlemew">{{ count }}</button>
</template>

<style>
.meow {
  color: aqua;
}
</style>
