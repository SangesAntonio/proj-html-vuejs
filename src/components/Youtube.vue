<template>
  <div class="text-center position-relative youtube">
    <img
      src="../assets/img/maxcoach-shape-12-150x150.png"
      class="cs-img-dot"
      alt=""
    />
    <img
      src="../assets/img/maxcoach-shape-05-150x150.png"
      class="dot-rigth"
      alt=""
    />
    <img
      src="../assets/img/artist-video-poster.jpg"
      class="w-50 shadow"
      alt=""
    />
    <img src="../assets/img/icon-youtube-play.png" class="logo-tube" alt="" />
  </div>
</template>

<script>
export default {
  name: "Youtube",
};
</script>

<style scoped land='scss'>
.youtube {
  margin-top: 160px;
  margin-bottom: 130px;
}
.logo-tube {
  max-width: 110px;
  height: 61px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.cs-img-dot {
  width: 200px;
  height: 200px;
  position: absolute;
  right: 18%;
  top: 65%;
  z-index: -1;
}
.dot-rigth {
  width: 200px;
  height: 200px;
  position: absolute;
  left: 23%;
  top: -20px;
  z-index: -1;
}
</style>