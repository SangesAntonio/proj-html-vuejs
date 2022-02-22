<template>
  <div id="app">
    <Header id="header" />
    <main>
      <section id="introduction-jumbotron">
        <Jumbotron />
      </section>
      <section id="artist-coaching" class="position-relative">
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
      <section id="blog-articles">
        <Blog />
      </section>
      <section id="event-list">
        <Events />
      </section>
    </main>
    <footer>
      <Banner id="newsletter-input" />
      <BottomFooter id="utils-link" />
    </footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Jumbotron from "./components/Jumbotron.vue";
import ArtistCoaching from "./components/ArtistCoaching.vue";
import Youtube from "./components/Youtube.vue";
import Slider from "./components/Slider.vue";
import CoursesStore from "./components/CoursesStore.vue";
import Blog from "./components/Blog.vue";
import Events from "./components/Events.vue";
import Banner from "./components/footer/Banner.vue";
import BottomFooter from "./components/footer/BottomFooter.vue";

export default {
  name: "App",
  components: {
    Header,
    Jumbotron,
    ArtistCoaching,
    Youtube,
    Slider,
    CoursesStore,
    Blog,
    Events,
    Banner,
    BottomFooter,
  },
};
</script>

<style lang="scss">
@import "./assets/scss/style.scss";
</style>
