<script>
export default {
  data() {
    return {
      visibility: false,
    }
  },
  methods: {
    changeVisibility: function() {
      this.visibility = !this.visibility
    }
  }
}
</script>
<template>
  <p v-if="visibility">P1</p>
  <p v-else>P2</p>
  <button @click="changeVisibility">visibility = {{ visibility }}</button>
</template>