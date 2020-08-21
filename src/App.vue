<template>
  <div id="app">
    <img
    src="./assets/pro.jpg"
    class="rounded-circle"
    width="20%"
    

    />
    <p>
      <br />
    </p>
    <hr />
    <HelloWorld msg="🌷 𝓐𝓡𝓐𝓨𝓐   𝓣𝓐𝓡𝓘𝓝 🌷" />
    <span class="users-list-date">💍 𝖂𝕬𝕹𝕰 💍</span>
    <br />
    <hr />
    <div class="row">
      <div class="col-4">
        <img src="https://lh3.googleusercontent.com/proxy/zjLAIHx_h9HjoMSLd7xAG2s2Q0wjzYkzp0KX4YOB5QKul7VAv8EgrWcbUt1FBHJVTi6yutJ4D_TdPiB3x2wwRI9rVzcPs86PBtkBaLz0M9co4lueAkUlJ-HddfXPFmj2I1E7Hg_GvBSn39U" class="rounded" width="50%" />
        <p>
          <br />
        </p>
        <Button />
      </div>
      <div class="col-4">
        <img src="https://www.ryt9.com/img/files/20190423/iqeca733ae6e4c1121bede1a07bcc7cf22.jpg" class="rounded" width="50%" />
        <p>
          <br />
        </p>
        <Button />
      </div>
      <div class="col-4">
        <img src="https://cms.dmpcdn.com/musicarticle/2015/12/09/6e620ebc-eee8-4a7b-b927-6355df37f989.jpg" class="rounded" width="50%" />
        <p>
          <br />
        </p>
        <Button />
      </div>
      <div class="col-4">
        <img src="https://i.pinimg.com/originals/2a/44/9d/2a449d1d96bc98b8c93db17b9fa2e0bb.png" class="rounded" width="50%" />
        <p>
          <br />
        </p>
        <Button />
      </div>
      <div class="col-4">
        <img src="https://cms.dmpcdn.com/musicarticle/2019/07/05/ac4f6723-669d-47b2-8cf1-eac458eb8dcc_original.jpg" class="rounded" width="50%" />
        <p>
          <br />
        </p>
        <Button />
      </div>
      <div class="col-4">
        <img src="https://sites.google.com/site/artist10fanclub/_/rsrc/1554473667055/prawati-phl-ngan-the-toy/DD35D087090D467B87DE118AA5303130.jpg?height=320&width=267" class="rounded" width="50%" />

        <p>
          <br />
        </p>
        <Button />
      </div>
    </div>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import Button from "./components/Button.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    Button,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #4e111b;
  margin-top: 60px;
}
</style>
