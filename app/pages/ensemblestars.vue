<template>
  <section class="ensemblestars">
    <div class="background">
      <div class="wave -one"></div>
      <div class="wave -two"></div>
      <div class="wave -three"></div>
      <div class="wave -four"></div>
      <div class="wave -five"></div>
      <h1 class="title">404</h1>
    </div>
    <div class="nannka">なんか要素</div>
    <div class="nannka">なんか要素</div>
    <div class="nannka">なんか要素</div>
    <div class="nannka">なんか要素</div>
    <div class="nannka">なんか要素</div>
    <div class="nannka">なんか要素</div>
    <div class="nannka">なんか要素</div>
    <div class="nannka">なんか要素</div>
    <div class="nannka">なんか要素</div>
  </section></template
>

<script>
export default {
  data() {
    return {};
  },
  mounted() {}
};
</script>

<style scoped>
.nannka {
  height: 200px;
}

html {
  background: #eee;
}

.background {
  width: 100%;
  height: 100%;
  background: lighten(#f0f4c3, 10%);
  position: fixed;
  overflow: hidden;
}

.wave {
  opacity: 0.4;
  position: absolute;
  top: 0%;
  left: 75%;
  background: #0af;
  width: 100%;
  height: 100vh;
  margin-left: -25%;
  margin-top: -25%;
  transform-origin: 50% 48%;
  border-radius: 59%;
  animation: drift 4000ms infinite linear;
}

.wave.-two {
  animation: drift 5000ms infinite linear;
  opacity: 0.1;
  background: yellow;
}

.wave.-three {
  animation: drift 6000ms infinite linear;
  background: rgb(124, 214, 210);
}

.wave.-four {
  animation: drift 7000ms infinite linear;
  background: rgb(96, 212, 183);
}

.wave.-five {
  animation: drift 8000ms infinite linear;
}

.box:after {
  content: "";
  display: block;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  z-index: 11;
}

@keyframes drift {
  from {
    transform: rotate(0deg);
  }
  from {
    transform: rotate(360deg);
  }
}

.title {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  z-index: 1;
  line-height: 300px;
  text-align: right;
  text-transform: uppercase;
  font-family: "Playfair Display", serif;
  text-shadow: 0 1px 0 rgba(black, 0.1);
  text-indent: 0.3em;
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 500px;
  color: #35495e;
  letter-spacing: 1px;
}
</style>
