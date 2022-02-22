<template>
  <div class="position-relative">
    <figure class="">
      <img :src="require(`../assets/img/${imag}`)" class="img-fluid" alt="" />
    </figure>

    <div class="px-4 over-cs">
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
.over-cs {
  border: 1px solid rgba(255, 255, 255, 0);
  background-color: white;
}
.over-cs:hover {
  border: 1px solid orange;
  transform: translate(-10, -15);
}
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