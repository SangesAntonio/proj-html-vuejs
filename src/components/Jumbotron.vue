<template>
  <div class="jumbotron">
    <img class="prima-left" src="../assets/img/artist-shape-03.png" alt="" />
    <img
      class="seconda-left"
      src="../assets/img/artist-hero-image-03.png"
      alt=""
    />
    <img
      class="terza-left"
      src="../assets/img/artist-hero-image-02.jpg"
      alt=""
    />
    <img
      class="quarta-left"
      src="../assets/img/artist-hero-image-01.jpg"
      alt=""
    />
    <img
      class="quinta-left"
      src="../assets/img/artist-shape-01-300x288.png"
      alt=""
    />
    <img class="sesta-rigth" src="../assets/img/artist-shape-04.png" alt="" />
    <img
      class="settima-rigth"
      src="../assets/img/artist-hero-image-04.jpg"
      alt=""
    />
    <img
      id="ottava-rigth"
      src="../assets/img/artist-shape-color-paint-bottom-right.png"
      alt=""
    />
  </div>
</template>

<script>
export default {
  name: "Jumbotron",
};
</script>

<style scoped lang='scss'>
.jumbotron {
  height: 80vh;
  background-color: #fbf9f6;
  position: relative;

  img {
    position: absolute;
  }

  .settima-rigth {
    right: 0px;
  }
  .sesta-rigth {
    right: 0px;
  }
  .prima-left {
  }
}
</style>