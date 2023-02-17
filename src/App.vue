<script>
export default {
  data() {
    return {
      cssClasses: "border: 5px solid red",
    };
  },
  methods: {},
};
</script>
<template>
  <p :style="cssClasses">text</p>
</template>
