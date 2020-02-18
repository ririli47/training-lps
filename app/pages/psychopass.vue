<template>
  <section class="psychopass">
    <ul>
      <li>NEWS</li>
      <li>THEATER</li>
      <li>STAFF & CAST</li>
      <li>INTRO & STORY</li>
      <li>CHARACTOR</li>
      <li>TRAILER</li>
      <li>Official Twitter</li>
      <li>TOP</li>
    </ul>
  </section></template
>

<script>
export default {
  data() {
    return {};
  },
  computed: {},
  methods: {}
};
</script>

<style scoped>
.psychopass {
  width: 100%;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

.psychopass > ul > li:hover {
  cursor: pointer;
  display: inline-block;
  animation: hurueru 0.1s infinite;
}

@keyframes hurueru {
  0% {
    transform: translate(0px, 0px) rotateZ(0deg);
  }
  25% {
    transform: translate(2px, 2px) rotateZ(1deg);
  }
  50% {
    transform: translate(0px, 2px) rotateZ(0deg);
  }
  75% {
    transform: translate(2px, 0px) rotateZ(-1deg);
  }
  100% {
    transform: translate(0px, 0px) rotateZ(0deg);
  }
}
</style>
