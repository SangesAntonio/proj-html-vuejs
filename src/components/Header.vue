<template>
  <div>
    <div class="timer text-center d-flex justify-content-center">
      <p>start tomorrow at 00:00:00...</p>
      <Button action="Get Ticket" childclass="px-4 py-0" />
    </div>
    <div class="container-sm my-4">
      <div class="bottom-header row">
        <div class="col-3">
          <img src="../assets/img/dark-logo.png" class="w-50" alt="Max Coach" />
        </div>
        <div class="col-6">
          <ul class="d-flex decoratione-cs">
            <li class="me-4" v-for="(item, index) in navbar" :key="index">
              <a href=""
                >{{ item.text }} <i class="ms-2 fa-solid fa-chevron-down"></i
              ></a>
            </li>
          </ul>
        </div>
        <div class="col-3">
          <i class="fa-brands fa-twitter"></i>
          <i class="fa-brands fa-facebook"></i>
          <i class="fa-brands fa-instagram"></i>
          <i class="fa-brands fa-linkedin"></i>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Button from "./Button.vue";
export default {
  name: "Header",
  components: {
    Button,
  },
  data() {
    return {
      navbar: [
        {
          text: "Home",
          url: "",
        },
        {
          text: "Pages",
          url: "",
        },
        {
          text: "Courses",
          url: "",
        },
        {
          text: "Features",
          url: "",
        },
        {
          text: "Blog",
          url: "",
        },
        {
          text: "Shop",
          url: "",
        },
      ],
    };
  },
};
</script>

<style scoped lang='scss'>
.timer {
  background-color: #f4f0ef;
}
.decoratione-cs {
  list-style-type: none;

  a {
    text-decoration: none;
    color: #1b1b1b;
    .fa-chevron-down {
      font-size: 8px;
    }
  }
}

.fa-brands {
  margin: 10px;
  font-size: 1.2rem;
  color: #797979;
}
</style>