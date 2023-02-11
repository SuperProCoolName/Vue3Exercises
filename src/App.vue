<script>
export default {
  data() {
    return {
      items: [1, -2, 3, -4, 5],
    }
  },
  methods: {

    }
}
</script>
<template>
  <div v-for="item in items">
    <p v-if="item >= 0">{{ item }}&nbsp;</p>
  </div>
</template>