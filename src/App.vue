<script>
export default {
  data() {
    return {
      isValid: true,
      isDisabled: true,
    };
  },
  methods: {
    setDone: function () {
      this.obj.hidden = !this.obj.hidden;
    },
  },
};
</script>
<template>
  <p :class="{ active: isValid, valid: isDisabled }">Задание 1</p>
</template>
<style>
.active {
  border: 5px solid red;
}
.valid {
  color: green;
}
</style>
