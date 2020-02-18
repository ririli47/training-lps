<template>
  <section class="container">
    <table class="table-auto">
      <thead>
        <tr>
          <th class="px-4 py-2">元サイトtitle</th>
          <th class="px-4 py-2">元サイトURL</th>
          <th class="px-4 py-2">サンプルリンク</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="item in items" :key="item.id">
          <td class="border px-4 py-2">{{ item.title }}</td>
          <td class="border px-4 py-2">
            <a :href="item.originLink" target="_blank">{{ item.originLink }}</a>
          </td>
          <td class="border px-4 py-2">
            <nuxt-link :to="item.sampleLink" target="_blank">{{
              item.sampleLink
            }}</nuxt-link>
          </td>
        </tr>
      </tbody>
    </table>
  </section>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          id: 0,
          title: "オンエア",
          originLink: "https://on-air-coly.com/",
          sampleLink: "onair"
        },
        {
          id: 1,
          title: "サイコパス",
          originLink: "https://psycho-pass.com/",
          sampleLink: "psychopass"
        },
        {
          id: 2,
          title: "鬼滅の刃",
          originLink: "https://kimetsu.com/anime/",
          sampleLink: "kimetu"
        },
        {
          id: 3,
          title: "あんさんぶるスターズ！",
          originLink: "https://ensemblestars-anime.com/",
          sampleLink: "ensemblestars"
        },
        {
          id: 4,
          title: "呪術廻戦",
          originLink: "https://jujutsukaisen.jp/",
          sampleLink: "jujutsukaisen"
        },
        {
          id: 5,
          title: "プロメア",
          originLink: "https://promare-movie.com/",
          sampleLink: "promare"
        },
        {
          id: 6,
          title: "天気の子",
          originLink: "https://tenkinoko.com/",
          sampleLink: "tenkinoko"
        },
        {
          id: 7,
          title: "ヒプノシスマイク",
          originLink: "https://hypnosismic.com/character/ikebukuro/",
          sampleLink: "hypnosismic"
        },
        {
          id: 8,
          title: "ドラえもん（フェリシモ）",
          originLink: "https://www.felissimo.co.jp/doraemon/",
          sampleLink: ""
        },
        {
          id: 9,
          title: "JPホールディングスグループ",
          originLink: "https://jphdgroup-recruit.jp/",
          sampleLink: ""
        },
        {
          id: 10,
          title: "約束のネバーランド",
          originLink: "https://neverland-anime.com/",
          sampleLink: ""
        },
        {
          id: 11,
          title: "PATRA",
          originLink: "https://patrainc.jp/",
          sampleLink: "patrainc"
        }
      ]
    };
  }
};
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
