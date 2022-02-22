<template>
  <div class="bg-cs position-relative">
    <img src="" alt="" />
    <TitleSections
      class="mx-auto"
      titleOne="Articles and Typs"
      titleTwo="Latest From The Blog"
    />
    <img
      src="../assets/img/maxcoach-shape-03.png"
      class="position-absolute img-back w-vw"
      alt=""
    />
    <img
      src="../assets/img/maxcoach-shape-05-100x100.png"
      class="position-absolute img-back left-30"
      alt=""
    />
    <div class="container-sm">
      <div class="row">
        <div class="col-3 index-cs position-relative">
          <CardBlogsm
            class="position-absolute top-25"
            imag="artist-blog-03-480x356.jpeg"
            title="Brush Strokes Energize
                    Trees in Paintings"
            views="603"
          />
        </div>
        <div class="col-6">
          <CardBlogxl class="mx-auto" />
        </div>
        <div class="col-3 index-cs position-relative">
          <CardBlogsm
            class="position-absolute top-10"
            imag="artist-blog-01-480x356.jpg"
            title="Pocket-Sized Notebooks
                    Hold Miniature Paintings"
            views="688"
          />
        </div>
        <div class="col-12 col-link text-center text-muted">
          <p>
            Get into details now?
            <a href="#" class="cs-link"
              >View all posts <i class="fa-solid fa-arrow-right"></i
            ></a>
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import TitleSections from "./TitleSections.vue";
import CardBlogsm from "./CardsBlog/CardBlogsm.vue";
import CardBlogxl from "./CardsBlog/CardBlogxl.vue";
export default {
  name: "Blog",
  components: {
    TitleSections,
    CardBlogsm,
    CardBlogxl,
  },
};
</script>

<style scoped lang='scss'>
.left-30 {
  left: 35%;
  top: 25%;
}
.top-25 {
  top: 25%;
}
.top-10 {
  top: 10%;
}
.img-back {
  z-index: 0;
}
.w-vw {
  width: 99vw;
}
.index-cs {
  z-index: 2;
}
.bg-cs {
  background-color: #faf8f6;
  padding-top: 100px;
}
.col-link {
  padding-top: 100px;
  padding-bottom: 50px;
}
.cs-link {
  color: #ef6f31;
  font-weight: bold;
  text-decoration: none;
  border-bottom: 1px solid rgb(197, 195, 195);
}
</style>