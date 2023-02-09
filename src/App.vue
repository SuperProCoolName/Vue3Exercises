<script>
export default {
  data() {
    return {
      isAdmin: true,
    }
  },
  methods: {
    toggle: function() {
      this.isAdmin = !this.isAdmin;
    }
  }
}
</script>
<template>
  <button @click="toggle">{{ isAdmin ? "give admin" : "take admin" }}</button><br>
  <p v-if="isAdmin">the user is admin</p>
  <p v-else>the user is NOT admin</p>
</template>