<template>
  <div>
    <div class="timer text-center d-flex justify-content-center">
      <p class="timer-text">
        Start TOMORROW! Our biggest event of the year...<i
          class="fa-regular fa-clock text-black px-3"
        ></i>
        <span class="text-black fw-bold">00 : 00 : 00</span>
      </p>
      <Button action="Get Ticket" childclass="px-4 py-1" class="ps-4" />
    </div>
    <div class="container-sm my-4">
      <div class="bottom-header row">
        <div class="col-3">
          <img src="../assets/img/dark-logo.png" class="w-50" alt="Max Coach" />
        </div>
        <div class="col-6">
          <ul class="d-flex decoratione-cs">
            <li class="me-4" v-for="(item, index) in navbar" :key="index">
              <a href="" class="over-cs"
                >{{ item.text }} <i class="ms-2 fa-solid fa-chevron-down"></i
              ></a>
            </li>
          </ul>
        </div>
        <div class="col-3 text-rig">
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
.text-rig {
  text-align: right;
}
.over-cs:hover {
  color: #ef6f31;
}
.timer {
  background-color: #f4f0ef;
  padding: 10px 0;
  .timer-text {
    color: #797979;
    font-weight: normal;
    font-size: 16px;
  }
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