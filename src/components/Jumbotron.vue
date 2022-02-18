<template>
  <div class="jumbotron">
    <img class="dots-left" src="../assets/img/artist-shape-03.png" alt="" />
    <img
      class="silouette-left"
      src="../assets/img/artist-hero-image-03.png"
      alt=""
    />
    <img
      class="abstract-left shadow-img"
      src="../assets/img/artist-hero-image-02.jpg"
      alt=""
    />
    <img
      class="monkey-left shadow-img"
      src="../assets/img/artist-hero-image-01.jpg"
      alt=""
    />
    <img
      class="background-rigth"
      src="../assets/img/artist-shape-01.png"
      alt=""
    />
    <img class="piuma-rigth" src="../assets/img/artist-shape-04.png" alt="" />
    <img
      class="abstract-rigth"
      src="../assets/img/artist-shape-05.png"
      alt=""
    />

    <img
      class="portrait-rigth shadow-img"
      src="../assets/img/artist-hero-image-04.jpg"
      alt=""
    />
    <TitleSections
      titleOne="Hello, Im Martin"
      titleTwo="Artist Coaching And Mentoring Migth be For You."
    />
  </div>
</template>

<script>
import TitleSections from "./TitleSections.vue";
export default {
  name: "Jumbotron",
  components: {
    TitleSections,
  },
};
</script>

<style scoped lang='scss'>
.jumbotron {
  height: 80vh;
  background-color: #fbf9f6;
  display: flex;
  position: relative;
  justify-content: center;
  align-items: center;

  .title-jumbo {
    width: 30%;

    .fancy-title {
      color: #029fcc;
      font-size: 2.6rem;
      font-family: "Dancing Script", cursive;
    }
    .second-title {
      font-weight: bold;
      font-size: 2.4rem;
      margin-bottom: 50px;
    }
  }

  img {
    position: absolute;
  }
  .portrait-rigth {
    right: 12%;
    top: 34%;
  }
  .piuma-rigth {
    right: 8%;
    top: 13%;
  }
  .dots-left {
    top: 150px;
    left: 1%;
  }
  .silouette-left {
    top: 50%;
    left: 25%;
  }
  .abstract-left {
    left: 17%;
    top: 13%;
  }
  .monkey-left {
    top: 55%;
    left: 8%;
  }
  .background-rigth {
    right: 7%;
    top: 0;
  }
  .abstract-rigth {
    right: 5%;
    top: 64%;
  }
}
.shadow-img {
  box-shadow: 0 0 20px -3px rgba(0, 0, 0, 0.589);
}
</style>