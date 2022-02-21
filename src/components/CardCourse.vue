<template>
  <div>
    <figure class="">
      <img :src="require(`../assets/img/${imag}`)" class="img-fluid" alt="" />
    </figure>

    <div class="px-4">
      <p class="price-color fw-bold">${{ price }}</p>
      <h4 class="">{{ title }}</h4>
      <div class="d-flex mt-4">
        <p class="fonts-cs pe-4 text-muted">
          <i class="fa-regular fa-file-lines pe-2"></i>{{ lessons }} lessons
        </p>
        <p class="text-muted fonts-cs">
          <i class="fa-regular fa-user pe-2"></i>{{ students }} students
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardCourse",
  props: ["imag", "price", "title", "lessons", "students"],
};
</script>

<style scoped lang='scss'>
h4 {
  font-size: 20px;
  font-weight: 500;
}
.price-color {
  color: #ef6f31;
  font-size: 18px;
}
.fonts-cs {
  font-size: 14px;
}
</style>