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
        <img src="./assets/boky.jpg" class="rounded" width="50%" />
        <p>
          <br />
        </p>
        <Button />
      </div>
      <div class="col-4">
        <img src="./assets/toy.jpg" class="rounded" width="50%" />
        <p>
          <br />
        </p>
        <Button />
      </div>
      <div class="col-4">
        <img src="./assets/Bright.jpg" class="rounded" width="50%" />
        <p>
          <br />
        </p>
        <Button />
      </div>
      <div class="col-4">
        <img src="./assets/Palmy.png" class="rounded" width="50%" />
        <p>
          <br />
        </p>
        <Button />
      </div>
      <div class="col-4">
        <img src="./assets/Ammy.jpg" class="rounded" width="50%" />
        <p>
          <br />
        </p>
        <Button />
      </div>
      <div class="col-4">
        <img src="./assets/polycat.jpg" class="rounded" width="50%" />

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
