<template>
  <section class="kimetu">
    <img src="http://placehold.jp/24/cc9999/993333/1500x1000.png" />
    <img src="http://placehold.jp/24/99cc99/993333/1500x1000.png" />
    <img src="http://placehold.jp/24/9999cc/993333/1500x1000.png" />
    <div id="target">hoge</div>
  </section></template
>

<script>
export default {
  data() {
    return {};
  },
  mounted() {
    const element = document.documentElement;
    const bottom = element.scrollHeight - element.clientHeight;
    scrollTo(0, bottom);

    console.log("bottom : " + bottom);
    setTimeout(function() {
      $("html, body").animate(
        {
          scrollTop: 0
        },
        3000
      );
    }, 2500);
  }
};
</script>

<style scoped>
.kimetu {
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: 100vw;
  background-size: cover;
}
</style>
