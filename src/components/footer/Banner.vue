<template>
  <div class="bg-banner position-relative">
    <img
      src="../../assets/img/artist-shape-color-paint-bottom-right.png"
      class="position-absolute left-img"
      alt=""
    />
    <img
      src="../../assets/img/artist-shape-color-paint-top-left-300x170.png"
      class="position-absolute rigth-img"
      alt=""
    />
    <div class="container-sm">
      <div class="row justify-content-between">
        <div class="col-3 position-banner">
          <h2 class="text-banner fs-1 px-2">Newsletter to get in touch</h2>
        </div>
        <div class="col-9 position-banner ps-4">
          <div class="text-right padding-80">
            <input
              type="email"
              class="email-input fs-4 pt-4 fw-normal w-75"
              placeholder="Your e-mail"
            />
            <a href=""
              ><i class="fa-solid fs-3 text-white fa-arrow-right"></i
            ></a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Banner",
};
</script>

<style scoped lang='scss'>
.bg-banner {
  margin-top: 80px;
  margin-bottom: 80px;
  width: 100%;
  height: 200px;
  background-color: #244186;

  .text-banner {
    color: white;
    font-family: "Times New Roman", Times, serif;
    text-align: right;
  }
}
.padding-80 {
  padding-left: 80px;
}
.position-banner {
  padding-top: 50px;
}
.email-input {
  background-color: #244186;
  border: none;
  border-bottom: 1px solid white;
  color: white;
}
.left-img {
  right: 0%;
  bottom: 0;
}
.rigth-img {
  left: 0;
  height: 100%;
}
img {
  overflow: hidden;
}
</style>