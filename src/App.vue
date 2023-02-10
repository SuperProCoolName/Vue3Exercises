<script>
export default {
  data() {
    return {
      visibility: true,
    }
  },
  methods: {
    toggle: function() {
      this.visibility = !this.visibility;
    }
  }
}
</script>
<template>
  <div v-if="visibility">
  <p>Paragraph 1</p>
  <p>Paragraph 2</p>
  <p>Paragraph 3</p>
  </div><br>
  <button @click="toggle">Toggle</button>
</template>