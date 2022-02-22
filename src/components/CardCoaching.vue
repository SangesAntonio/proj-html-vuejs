<template>
  <div class="card border-0">
    <img :src="require(`../assets/img/${imag}`)" class="card-img-top" alt="" />
    <div class="card-body">
      <h5 class="card-title">{{ title }}</h5>
      <p class="card-text text-muted">
        {{ info }}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "cardCoaching",
  props: ["imag", "title", "info"],
};
</script>

<style scoped lang='scss'>
img {
  width: 120px;
  height: auto;
}
</style>