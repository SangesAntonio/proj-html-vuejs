<template>
  <div class="container-cs position-relative">
    <div class="row">
      <div class="col-4 text-address">
        <h3 class="text-black">Address</h3>
        <p>382 NE 191st St # 87394 Miami, FL 33179-3899</p>
        <p>+1(305) 547-9909 (9am - 5pm EST, Monday - Friday)</p>
        <p>support@maxcoach.com</p>
        <div class="d-flex w-50 justify-content-between text-muted">
          <i class="fa-brands fa-facebook"></i>
          <i class="fa-brands fa-twitter"></i>
          <i class="fa-brands fa-instagram"></i>
          <i class="fa-brands fa-linkedin"></i>
        </div>
      </div>
      <div class="col-4">
        <div class="row">
          <div class="col-6 explore">
            <h3 class="text-black pb-2">Explore</h3>
            <ul>
              <li><a href="#">Start here</a></li>
              <li><a href="#">Success sory</a></li>
              <li><a href="#">Blog</a></li>
              <li><a href="#">Courses</a></li>
              <li><a href="#">Contact us</a></li>
            </ul>
          </div>
          <div class="col-6 explore">
            <h3 class="text-black pb-2">Information</h3>
            <ul>
              <li><a href="#">Membership</a></li>
              <li><a href="#">purchase guide</a></li>
              <li><a href="#">Privacy policy</a></li>
              <li><a href="#">terms of services</a></li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-4">
        <h3>instagram <a href="#" class="cs-color">@maxcoach</a></h3>
        <div class="d-flex">
          <div class="img-square">
            <img
              src="../../assets/img/artist-blog-03-480x356.jpeg"
              class=""
              alt=""
            />
          </div>
          <div class="img-square">
            <img
              src="../../assets/img/artist-event-03-250x300.jpg"
              class=""
              alt=""
            />
          </div>
          <div class="img-square">
            <img
              src="../../assets/img/artist-event-02-250x300.jpg"
              class=""
              alt=""
            />
          </div>
        </div>
      </div>
      <div class="col-12 text-center position-relative">
        <p class="copyrigth">
          <i class="far fa-copyright"></i>2020 Maxcoach. All Rigth Reserved.
        </p>
        <div class="circle-arrow">
          <a href="#header"><i class="fa-solid fa-arrow-up"></i></a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Bottomfooter",
};
</script>

<style scoped lang='scss'>
.circle-arrow {
  width: 70px;
  height: 70px;
  border-radius: 50%;
  background-color: #ef6f31;
  display: flex;
  justify-content: center;
  align-items: center;
  position: absolute;
  right: 0;
  bottom: 40%;
  font-size: 25px;

  a {
    color: white;
    text-decoration: none;
  }
}
.copyrigth {
  color: rgb(170, 167, 167);
  margin-top: 100px;
  margin-bottom: 70px;
  font-size: 13px;
}
.img-square {
  padding: 10px;
  width: 130px;
  height: 130px;
}
img {
  width: 100%;
  height: 100%;
}
.cs-color {
  font-size: 14px;
  color: #ef6f31;
}
.container-cs {
  width: 80%;
  margin: 0 auto;
}
h3 {
  font-size: 16px;
}
.text-address {
  font-weight: 200;
  color: rgb(98, 98, 98);
  font-size: 13px;
}
.fa-brands {
  font-size: 25px;
}
.explore {
  ul {
    list-style-type: none;
    padding: 0;
    li {
      padding-bottom: 10px;
      a {
        font-size: 13px;
        text-decoration: none;
        color: rgb(98, 98, 98);
      }
    }
  }
}
</style>