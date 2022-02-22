<template>
  <div class="container-sm">
    <div class="row gy-3 mb-4">
      <div class="col-12">
        <TitleSections
          class="mx-auto pt-4 mt-4"
          titleOne="Upcoming Events"
          titleTwo="Let's work Together"
        />
      </div>
      <CardEvent
        class="col-6 p-4"
        v-for="(event, index) in events"
        :key="index"
        :class="index < 2 ? '' : 'flex-row-reverse'"
        :imag="event.imag"
        :date="event.date"
        :title="event.title"
        :location="event.location"
      />
    </div>
  </div>
</template>

<script>
import CardEvent from "./CardsEvent/CardEvent.vue";
import TitleSections from "./TitleSections.vue";
export default {
  name: "Events",
  components: {
    CardEvent,
    TitleSections,
  },
  data() {
    return {
      classe: "",
      events: [
        {
          imag: "artist-event-04-250x300.jpg",
          date: "Nov 22, 2020",
          title: "Storytelling Workshop",
          location: "Texas, US",
        },
        {
          imag: "artist-event-03-250x300.jpg",
          date: "Oct 10, 2020",
          title: "Painting Art Contest 2020",
          location: "New York, US",
        },
        {
          imag: "artist-event-02-250x300.jpg",
          date: "Nov 23, 2020",
          title: "International Art Fair 2020",
          location: "Hamburg, Germany",
        },
        {
          imag: "artist-event-01-250x300.jpg",
          date: "Dec 15, 2020",
          title: "Storytelling Workshop",
          location: "Illinois, US",
        },
      ],
    };
  },
};
</script>

<style scoped lang='scss'>
</style>