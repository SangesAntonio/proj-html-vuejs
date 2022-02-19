<template>
  <div class="text-center title-jumbo">
    <h1 :class="className" class="fancy-title">{{ titleOne }}</h1>
    <h1 :class="className" class="second-title">
      {{ titleTwo }}
    </h1>
  </div>
</template>

<script>
export default {
  name: "titleSections",
  props: ["titleOne", "titleTwo", "className"],
  components: {},
};
</script>

<style scoped lang='scss'>
.title-jumbo {
  width: 600px;

  .fancy-title {
    color: #029fcc;
    font-size: 2.6rem;
    font-family: "Dancing Script", cursive;
  }
  .second-title {
    font-weight: bold;
    font-size: 2.4rem;
    margin-bottom: 50px;
  }
}
</style>