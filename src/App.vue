<script>
export default {
  data() {
    return {
      day: "if you see this then something went wrong",
    }
  },
  methods: {
    dayOfTheWeek: function() {
    this.day = new Date().getDay();
  },
}
}
</script>
<template>
  <button @click="dayOfTheWeek">Click to reveal paragraph</button><br>
  <p v-if="this.day === 1">Monday</p>
  <p v-if="this.day === 2">Tuesday</p>
  <p v-if="this.day === 3">Wednesday</p>
  <p v-if="this.day === 4">Thursday</p>
  <p v-if="this.day === 5">Friday</p>
  <p v-if="this.day === 6">Saturday</p>
  <p v-if="this.day === 0">Sunday</p>
</template>