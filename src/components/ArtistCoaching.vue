<template>
  <div class="row mt-4">
    <div class="col d-flex justify-content-center">
      <TitleSections
        titleOne="ArtistCoaching"
        titleTwo="I understand what it takes to create.
            I can help you with"
        className="fw-normal"
      />
    </div>
    <div class="col-12 d-flex justify-content-center pt-3">
      <CardCoaching
        v-for="(card, index) in cards"
        :key="index"
        :imag="card.img"
        :title="card.title"
        :info="card.paragraph"
      />
    </div>
  </div>
</template>

<script>
import TitleSections from "./TitleSections.vue";
import CardCoaching from "./CardCoaching.vue";
export default {
  name: "ArtistCoaching",
  components: {
    TitleSections,
    CardCoaching,
  },
  data() {
    return {
      cards: [
        {
          img: "artist-box-image-01.png",
          title: "Online coures",
          paragraph:
            "Online art coaching now offers you a very powerful way to redesign your artist mind.",
        },
        {
          img: "artist-box-image-02.png",
          title: "One to One",
          paragraph:
            "Getting the necessary clarity about the current state to help you improve your ability.",
        },
        {
          img: "artist-box-image-03.png",
          title: "Anywhere",
          paragraph:
            "Access to valuable and portable program which allow you to setup and live anywhere you want.",
        },
        {
          img: "artist-box-image-04.png",
          title: "On time",
          paragraph:
            "Punctuality is our top priority because it's an essential criteria to assess a program quality.",
        },
      ],
    };
  },
};
</script>

<style scoped lang='scss'>
</style>