<template>
  <section class="jujutsukaisen">
    <h1 id="title">Mousemove!</h1>
    <span
      id="background"
      :style="{ backgroundImage: 'url(images/jujutsukaisen/back.jpg)' }"
    ></span></section
></template>

<script>
export default {
  data() {
    return {};
  },
  mounted() {
    //#titleを取得
    let title = document.getElementById("title");
    //#backgroundを取得
    let background = document.getElementById("background");

    document.addEventListener("mousemove", event => {
      //X座標(値は適宜調整)
      var x = Math.round(event.pageX / 100);
      //Y座標(値は適宜調整)
      var y = Math.round(event.pageY / 100);

      //#titleのX軸・Y軸を設定
      title.style.marginLeft = -x + "px";
      title.style.marginTop = -y + "px";

      //#backgroundのX軸・Y軸を設定
      background.style.marginLeft = x + "px";
      background.style.marginTop = y + "px";
    });
  }
};
</script>

<style scoped>
section {
  position: relative;
  width: 100%;
  height: 100vh;
  overflow: hidden;
}

#title {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  color: #cccccc;
  font-size: 3em;
  font-weight: bolder;
  z-index: 1;
}

#background {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  display: block;
  width: calc(100% + 40px);
  height: calc(100% + 40px);
  background-image: url(https://into-the-program.com/uploads/3169.jpg);
  background-repeat: no-repeat;
  background-size: cover;
}
</style>
