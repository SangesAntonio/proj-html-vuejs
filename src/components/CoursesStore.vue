<template>
  <div class="container-cs">
    <div class="row">
      <div class="col-12 pt-4">
        <TitleSections
          class="mx-auto mt-4"
          titleOne="Artist coaching"
          titleTwo="Latest Online Course"
          className=""
        />
      </div>
      <div class="col-12">
        <div class="row gy-3">
          <CardCourse
            class="col-3 p-3"
            v-for="(course, index) in courses"
            :key="index"
            :imag="course.imag"
            :price="course.price"
            :title="course.title"
            :lessons="course.lessons"
            :students="course.students"
          />
        </div>
      </div>
      <div class="col-12 text-center">
        <Button
          class="mx-auto"
          action="view all courses "
          icon="fa-solid fa-arrow-right"
          childclass="btn-clear px-4 py-3"
        />
      </div>
    </div>
  </div>
</template>

<script>
import TitleSections from "./TitleSections.vue";
import CardCourse from "./CardCourse.vue";
import Button from "./Button.vue";
export default {
  name: "CoursesStore",
  components: {
    TitleSections,
    CardCourse,
    Button,
  },
  data() {
    return {
      courses: [
        {
          imag: "artist-course-08-480x480.jpg",
          price: "18.00",
          title: "The Acrylic Painting Academy",
          lessons: "4",
          students: "50",
        },
        {
          imag: "artist-course-07-480x480.jpg",
          price: "21.00",
          title: "Drawing and Shading: Complete Course",
          lessons: "14",
          students: "50",
        },
        {
          imag: "artist-course-06-480x480.jpg",
          price: "19.00",
          title: "The Color Theory For Digital Artist",
          lessons: "7",
          students: "50",
        },
        {
          imag: "artist-course-05-480x480.jpg",
          price: "35.00",
          title: "Ultimate Guide to Digital Sketching for Beginner",
          lessons: "14",
          students: "50",
        },
        {
          imag: "artist-course-04-480x480.jpg",
          price: "19.00",
          title: "Portrait Drawing The Smart Way",
          lessons: "2",
          students: "50",
        },
        {
          imag: "artist-course-03-480x480.jpg",
          price: "19.00",
          title: "Mastering Watercolor Painting From Beginner",
          lessons: "9",
          students: "50",
        },
        {
          imag: "artist-course-02-480x480.jpg",
          price: "25.00",
          title: "The Art & Science of Drawing",
          lessons: "4",
          students: "50",
        },
        {
          imag: "artist-course-01-480x480.jpg",
          price: "22.00",
          title: "The Colored Pancil Drawing Course",
          lessons: "6",
          students: "50",
        },
      ],
    };
  },
};
</script>

<style scoped lang='scss'>
.container-cs {
  width: 75%;
  margin: 0 auto;
}
</style>