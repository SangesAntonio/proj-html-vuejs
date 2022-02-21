<template >
  <div class="container-cs">
    <div class="row justify-content-center bg-color">
      <div class="col-12">
        <div class="row justify-content-center">
          <TitleSections
            titleOne="Testimonials"
            titleTwo="Why do people love me"
            className="fw-normal"
          />
        </div>
      </div>
      <div class="row mt-4 justify-content-between p-4">
        <CardSlide
          class="col-3 hide-card"
          v-for="(card, index) in testimonials"
          :key="index"
          :class="{ activeslide: setCurrentImg(index) }"
          :title="card.titleOne"
          :paragraph="card.parag"
          :imag="card.imag"
          :name="card.name"
          :role="card.role"
        />
        <div class="col-12 d-flex justify-content-center mt-4">
          <div
            v-for="(card, index) in testimonials"
            :key="index"
            class="dots mx-3"
            :class="{ active: setCurrentImg(index) }"
            @click="getCurrentIndex(index)"
          ></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import TitleSections from "./TitleSections.vue";
import CardSlide from "./CardSlide.vue";
export default {
  name: "Slide",
  components: {
    TitleSections,
    CardSlide,
  },
  data() {
    return {
      testimonials: [
        {
          titleOne: "High level of efficiency and scientific teaching methods",
          parag:
            "i am free to learn at my own pace, follow my own schedule and choose the subjectI want to learn from the syllabus. Great study portal for people like me.",
          imag: "artist-testimonial-avatar-04.jpg",
          name: "Mina Hallace",
          role: "freelancer",
        },
        {
          titleOne:
            "Professional team of specialists and passionate mentors at reach",
          parag:
            "I need to get a certification for English proficiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.",
          imag: "artist-testimonial-avatar-03.jpg",
          name: "Madlei Pondor",
          role: "IT specialist",
        },
        {
          titleOne: "It's a choice of quality for people with special needs",
          parag:
            "i ma very strict person so I require everything to be organized and neat. Then, I'll be able to make things right and shine. MaxCoach guys just got me.",
          imag: "artist-testimonial-avatar-02.jpg",
          name: "Florence Themes",
          role: "Multimedia Admin",
        },
      ],
      currentIndex: "",
    };
  },
  methods: {
    getCurrentIndex(index) {
      this.currentIndex = index;
    },
    setCurrentImg(index) {
      return this.currentIndex === index;
    },
  },
};
</script>

<style scoped lang='scss'>
.container-cs {
  width: 90%;
  margin: 0 auto;
}
.bg-color {
  background-color: #faf8f6;
}
.hide-card {
  opacity: 0.5;
}
.activeslide {
  opacity: 1;
}
.dots {
  height: 10px;
  width: 10px;
  background-color: rgb(202, 196, 196);
  border-radius: 50%;
  cursor: pointer;
  margin-top: 100px;
  margin-bottom: 100px;
}
.active {
  background-color: rgb(34, 33, 33);
  height: 13px;
  width: 13px;
}
</style>