<template>
  <div>
    <button type="button" :class="childclass" class="btn">{{ action }}</button>
  </div>
</template>

<script>
export default {
  name: "Button",
  props: ["action", "childclass"],
};
</script>

<style scoped land='scss'>
.btn {
  font-size: 15px;
  font-weight: bold;
  margin-left: 20px;
  color: white;
  background-color: #ef6f31;
}
</style>