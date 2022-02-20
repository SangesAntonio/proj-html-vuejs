<template>
  <div class="bg-white">
    <h5 class="fw-bold mb-3">{{ title }}</h5>
    <p class="lh-lg text-secondary">{{ paragraph }}</p>
    <div class="card mb-3 border-0" style="max-width: 540px">
      <div class="row g-0 align-items-center">
        <div class="col-md-3">
          <img
            :src="require(`../assets/img/${imag}`)"
            class="img-fluid w-75 rounded-cs"
            alt="..."
          />
        </div>
        <div class="col-md-8">
          <div class="card-body">
            <h5 class="card-title">{{ name }}</h5>

            <p class="card-text">
              <small class="">/{{ role }}</small>
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardSlide",
  props: ["title", "paragraph", "imag", "name", "role"],
};
</script>

<style scoped lang='scss'>
.rounded-cs {
  border-radius: 50%;
}
</style>