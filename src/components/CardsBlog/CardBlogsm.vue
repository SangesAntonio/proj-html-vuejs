<template>
  <div class="back-shadow">
    <figure class="">
      <img
        :src="require(`../../assets/img/${imag}`)"
        class="img-fluid"
        alt=""
      />
    </figure>

    <div class="px-4 bg-white">
      <p class="price-color text-muted">ARTIST</p>
      <h4 class="">{{ title }}</h4>
      <div class="d-flex mt-4">
        <p class="fonts-cs pe-4 text-muted">
          <i class="fa-regular fa-calendar pe-2"></i> May 15, 2020
        </p>
        <p class="text-muted fonts-cs pb-4">
          <i class="fa-regular fa-eye pe-2"></i>{{ views }} views
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardBlogxl",
  props: ["imag", "title", "views"],
};
</script>

<style scoped lang='scss'>
h4 {
  font-size: 20px;
  font-weight: 500;
}
.price-color {
  font-size: 18px;
}
.fonts-cs {
  font-size: 14px;
}
.back-shadow {
  box-shadow: 0 0 100px 1px rgb(172, 170, 170);
  z-index: 2;
}
</style>