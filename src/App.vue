<script>
export default {
  data() {
    return {
      visibility: false,
    }
  },
  methods: {
    changeVisibilityToTrue: function() {
      this.visibility = true;
    },
    changeVisibilityToFalse: function() {
      this.visibility = false;
    }
  }
}
</script>
<template>
  <button v-if="!visibility" @click="changeVisibilityToTrue">Show text</button>
  <button v-else @click="changeVisibilityToFalse">Hide text</button><br>
  <p v-if="visibility">Some text</p>
</template>