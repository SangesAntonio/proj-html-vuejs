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
      <section id="youtube">
        <Youtube />
      </section>
      <section id="testimonials">
        <Slider />
      </section>
      <section id="online-courses">
        <CoursesStore />
      </section>
      <section id="blog-articles"></section>
    </main>
    <footer>ciao</footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Jumbotron from "./components/Jumbotron.vue";
import ArtistCoaching from "./components/ArtistCoaching.vue";
import Youtube from "./components/Youtube.vue";
import Slider from "./components/Slider.vue";
import CoursesStore from "./components/CoursesStore.vue";

export default {
  name: "App",
  components: {
    Header,
    Jumbotron,
    ArtistCoaching,
    Youtube,
    Slider,
    CoursesStore,
  },
};
</script>

<style lang="scss">
@import "./assets/scss/style.scss";
</style>
