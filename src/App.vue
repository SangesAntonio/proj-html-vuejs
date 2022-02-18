<template>
  <div id="app">
    <Header class="" />
    <main>
      <Jumbotron />
    </main>
    <footer>ciao</footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Jumbotron from "./components/Jumbotron.vue";
export default {
  name: "App",
  components: {
    Header,
    Jumbotron,
  },
};
</script>

<style lang="scss">
@import "./assets/scss/style.scss";
</style>
