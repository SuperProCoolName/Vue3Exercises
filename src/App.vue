<script>
export default {
  data() {
    return {

    }
  },
  methods: {
    alyarm: function() {
      alert(`This will only be shown once`);
    }
  }
}
</script>
<template>
  <a href.prevent="https://github.com/SuperProCoolName/Vue3Exercises" target="_blank">Link</a><br>
  <button @click.once="alyarm">Button</button>
</template>