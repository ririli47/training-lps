<template>
  <section class="patrainc">
    <div class="nannka">なんか要素</div>
    <div class="nannka">なんか要素</div>
    <div class="nannka">なんか要素</div>
    <div class="nannka">なんか要素</div>
    <div class="nannka">なんか要素</div>
    <div class="nannka">なんか要素</div>
    <div class="nannka">なんか要素</div>
    <div class="nannka">なんか要素</div>
    <div class="nannka">なんか要素</div>

    <img class="img" src="/images/foreground-top-fence.png" /></section
></template>

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
.patrainc {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.img {
  position: fixed;
  bottom: 0;
}

.nannka {
  height: 200px;
}
</style>
