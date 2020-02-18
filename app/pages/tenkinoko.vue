<template>
  <section class="tenkinoko">
    <div class="side-left">
      <ul>
        <li><a href="#news">NEWS</a></li>
        <li><a href="#tehater">THEATER</a></li>
        <li><a href="#staff">STAFF & CAST</a></li>
        <li><a href="#intro">INTRO & STORY</a></li>
        <li><a href="#charactor">CHARACTOR</a></li>
        <li><a href="#trailer">TRAILER</a></li>
        <li><a href="#twitter">Official Twitter</a></li>
        <li><a href="#top">TOP</a></li>
      </ul>
    </div>
    <div class="side-right">
      <div class="contents" id="news">NEWS</div>
      <div class="contents" id="tehater">THEATER</div>
      <div class="contents" id="staff">STAFF & CAST</div>
      <div class="contents" id="intro">INTRO & STORY</div>
      <div class="contents" id="charactor">CHARACTOR</div>
      <div class="contents" id="trailer">TRAILER</div>
      <div class="contents" id="twitter">Official Twitter</div>
      <div class="contents" id="top">TOP</div>
    </div>
  </section></template
>

<script>
export default {
  data() {
    return {};
  },
  mounted() {
    $(function() {
      $('a[href^="#"]').click(function() {
        var speed = 500;
        var href = $(this).attr("href");
        var target = $(href == "#" || href == "" ? "html" : href);
        var position = target.offset().top;
        $("html, body").animate({ scrollTop: position }, speed, "swing");
        return false;
      });
    });
  }
};
</script>

<style scoped>
.tenkinoko {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.side-left {
  text-align: left;
  position: fixed;
  top: 20%;
  left: 0;
  flex: 1;
}
.side-right {
  flex: 3;
  margin-left: 30%;
}

.side-left > ul > li {
  font-size: 40px;
}

.side-left > ul > li:hover {
  cursor: pointer;
  display: inline-block;
  color: red;
}
.contents {
  height: 1000px;
  font-size: 200px;
}

#news {
  background-color: #ff0000;
}
#tehater {
  background-color: #e30f01;
}

#staff {
  background-color: #724805;
}

#intro {
  background-color: #127909;
}

#charactor {
  background-color: #0d5953;
}

#trailer {
  background-color: #062fb5;
}

#twitter {
  background-color: #0322d5;
}

#top {
  background-color: #0010ff;
}
</style>
