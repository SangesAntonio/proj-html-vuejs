<template>
  <div class="position-relative bg-over">
    <figure class="">
      <img
        :src="require(`../../assets/img/artist-blog-02-500x680.jpg`)"
        class="img-fluid"
        alt=""
      />
    </figure>

    <div class="position-absolute info-card">
      <p class="artist-s">ARTIST</p>
      <h4 class="">
        Connection Between Self- <br />
        Portraits and Identity
      </h4>
      <div class="d-flex mt-4">
        <p class="fonts-cs pe-4">
          <i class="fa-regular fa-calendar"></i> May 20, 2020
        </p>
        <p class="fonts-cs"><i class="fa-regular fa-eye"></i> 560 view</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardBlogxl",
};
</script>

<style scoped lang='scss'>
.bg-over {
  background-color: black;
  width: 500px;
}
figure {
  width: 500px;
  img {
    opacity: 0.8;
  }
}
h4 {
  font-size: 34px;
  font-weight: 700;
}
.artist-s {
  font-size: 18px;
}
.fonts-cs {
  font-size: 14px;
}
.info-card {
  bottom: 5%;
  color: white;
  width: 100%;
  padding: 20px 20px;
}
</style>