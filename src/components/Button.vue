<template>
  <div>
    <button type="button" :class="childclass" class="btn">
      {{ action }} <i :class="icon"></i>
    </button>
  </div>
</template>

<script>
export default {
  name: "Button",
  props: ["action", "childclass", "icon"],
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
.btn:hover {
  background-color: #5688f3;
  color: white;
}
.btn-clear {
  background-color: #fdf0ea;
  color: #ef6f31;
}
</style>