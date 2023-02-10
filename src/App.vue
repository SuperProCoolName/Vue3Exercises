<script>
export default {
  data() {
    return {
      arr: ['x', 'y', 'z'],
    }
  },
  methods: {

    }
}
</script>
<template>
  <p v-for="(elem, key) in arr">{{ key }}:&nbsp {{ elem }}</p>
</template>
