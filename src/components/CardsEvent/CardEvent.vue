<template>
  <div class="row" :class="{ 'flex-row-reverse': classRow }">
    <div class="col-5">
      <img :src="require(`../../assets/img/${imag}`)" alt="" />
    </div>
    <div class="col-7 text-card">
      <p class="text-muted">{{ date }}</p>
      <h5 class="mt-3 mb-3">{{ title }}</h5>
      <p class="text-muted">
        <i class="pe-2 fa-solid fa-location-dot"></i>{{ location }}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardEvent",
  props: ["imag", "date", "title", "location", "classRow"],
};
</script>

<style scoped lang='scss'>
.text-card {
  padding-top: 100px;
  padding-left: 50px;
}
</style>