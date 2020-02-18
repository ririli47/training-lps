<template>
  <section
    class="onair"
    :style="{ backgroundImage: 'url(' + getBackgroundImagepath() + ')' }"
  ></section
></template>

<script>
export default {
  data() {
    return {
      backgroundImages: ["kawaii.png", "kizunaai.png", "simple.jpeg"]
    };
  },
  computed: {},
  methods: {
    getRandInt(max) {
      return Math.floor(Math.random() * Math.floor(max));
    },
    getBackgroundImagepath() {
      return "../images/onair/" + this.backgroundImages[this.getRandInt(3)];
    }
  }
};
</script>

<style scoped>
.onair {
  width: 100vw;
  height: 100vh;
  background-size: contain;
}
</style>
