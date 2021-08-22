<template>
  <h1>Events For Good</h1>
  <div class="events">
       <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from "@/components/EventCard.vue";

export default {
  name: "EventList",
  components: {
    EventCard
  },
   data() {
    return {
      events: [
        {
        id: 5928101,
        category: "animal welfare",
        title: 'Cat Adoption Day',
        description: 'find your new frined ',
        location: 'New York',
        date: 'January 23, 2021',
        time: '15:00',
        petsAllowed: true,
        organizers: 'aproko'
      },
       {
        id: 5928102,
        category: "animal welfare",
        title: 'Cat Adoption Day',
        description: 'find your new frined ',
        location: 'new york',
        date: 'January 23, 2021',
        time: '15:00',
        petsAllowed: true,
        organizers: 'aproko'
      },
       {
        id: 5928103,
        category: 'animal welfare',
        title: 'Cat Adoption Day',
        description: 'find your new frined ',
        location: 'new york',
        date: 'January 23, 2021',
        time: '15:00',
        petsAllowed: true,
        organizers: 'aproko'
      }
      ]
    }
      
  }
      
};


</script>
<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>