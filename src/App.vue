<template>
  <div id="app">
    <Header class="" />
    <main>
      <section id="introduction-jumbotron">
        <Jumbotron />
      </section>
      <section id="artist-coaching">
        <ArtistCoaching />
      </section>
      <section></section>
    </main>
    <footer>ciao</footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Jumbotron from "./components/Jumbotron.vue";
import ArtistCoaching from "./components/ArtistCoaching.vue";
export default {
  name: "App",
  components: {
    Header,
    Jumbotron,
    ArtistCoaching,
  },
};
</script>

<style lang="scss">
@import "./assets/scss/style.scss";
</style>
