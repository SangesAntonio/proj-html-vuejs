<template>
  <div class="text-center title-jumbo">
    <h1 :class="{ className }" class="fancy-title">{{ titleOne }}</h1>
    <h1 :class="{ className }" class="second-title">
      {{ titleTwo }}
    </h1>
    <Button action="Get started today" childclass="px-5 py-3" />
  </div>
</template>

<script>
import Button from "./Button.vue";

export default {
  name: "titleSections",
  props: ["titleOne", "titleTwo", " className"],
  components: {
    Button,
  },
};
</script>

<style scoped lang='scss'>
.title-jumbo {
  width: 30%;

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