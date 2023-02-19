<script>
export default {
  data() {
    return {
      isDisabled: false,
    };
  },
  methods: {},
};
</script>
<template>
  <input
    type="checkbox"
    :checked="isDisabled"
    @click="($event) => (this.isDisabled = !this.isDisabled)"
  />
  &nbsp;
  <button
    v-bind:disabled="!isDisabled"
    @click="($event) => (this.isDisabled = !this.isDisabled)"
  >
    {{ isDisabled ? "input is enabled" : "input is disabled" }}
  </button>
</template>
