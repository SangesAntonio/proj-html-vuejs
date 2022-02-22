<template>
  <div class="row justify-content-center gx-0">
    <img
      src="../assets/img/maxcoach-shape-03.png"
      class="position-absolute img-back"
      alt=""
    />
    <img
      src="../assets/img/maxcoach-shape-13-100x100.png"
      class="position-absolute sand"
      alt=""
    />
    <div class="col-12">
      <TitleSections
        class="mx-auto"
        titleOne="ArtistCoaching"
        titleTwo="I understand what it takes to create.
            I can help you with"
        className="fw-normal"
      />
    </div>
    <div class="col-10">
      <div class="row justify-content-center">
        <CardCoaching
          class="col-3"
          v-for="(card, index) in cards"
          :key="index"
          :imag="card.img"
          :title="card.title"
          :info="card.paragraph"
        />
      </div>
    </div>
    <div class="container-sm mt-4">
      <div class="row justify-content-center gx-0">
        <div class="col-4 text-center">
          <img
            src="../assets/img/artist-quote-icon.png"
            class="img-fluid"
            alt=""
          />
          <h1 class="lh-base fw-bold w-75 m-auto pt-4">
            I coach and mentor visual artists, like <br />
            you, to Create Like <br />
            You Mean It
          </h1>
          <h1 class="fancy pt-4">Martin Garrix</h1>
        </div>
        <div class="col-4 pt-4">
          <p class="lh-lg pt-5 paragraph">
            As a coach and mentor, my ultimate goal is to motivate visual
            artists toward inspired action. I helpP you get you back on track to
            being the productive, creative, meaningful and authentic artist you
            truly want to be.l support artists in crafting and living a creative
            life as well as feeling good about themselves and their art. <br />
            <br />
            As an artist and an educator for nearly 30 years, I understand what
            it takes to create.
          </p>
          <Button action="Get started Today" childclass="btn-clear p-3  px-4" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import TitleSections from "./TitleSections.vue";
import CardCoaching from "./CardCoaching.vue";
import Button from "./Button.vue";

export default {
  name: "ArtistCoaching",
  components: {
    TitleSections,
    CardCoaching,
    Button,
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
.img-back {
  z-index: 2;
  opacity: 0.3;
}
.sand {
  width: 200px;
  height: auto;
  right: 0px;
  top: 20%;
}
.fancy {
  font-family: "Festive", cursive;
  color: #029fcc;
}
h1 {
  font-size: 2.9rem;
}
.paragraph {
  text-align: start;
  color: rgb(100, 99, 99);
  font-size: 1.1rem;
}
</style>