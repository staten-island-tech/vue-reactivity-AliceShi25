<script>
export default {
  data() {
    return {
      message: "mewmew",
      sameww: "meow",
      count: 0,
      text: "",
      lyuvee: true,
    };
  },
  methods: {
    littlemew() {
      // update component state
      this.count++;
    },
    onInput(e) {
      this.text = e.target.value;
    },
    toggle() {
      this.lyuvee = !this.lyuvee;
    },
  },
};
</script>

<template>
  <h1 v-bind:class="sameww">{{ message }}</h1>
  <button @click="littlemew">{{ count }}</button>
  <button @click="toggle">
    <h1 v-if="lyuvee">heweeoewo</h1>
    <h1 v-else>hehiajak</h1>
  </button>
  <input :value="text" @input="onInput" placeholder="Type here" />
  <p>{{ text }}</p>
</template>

<style scoped>
.meow {
  color: aqua;
}
</style>
