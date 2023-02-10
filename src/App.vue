<script>
export default {
  data() {
    return {
      visibility: false,
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
  <p v-show="visibility">Paragraph 1</p><br>
  <button @click="toggle">Toggle</button>
</template>