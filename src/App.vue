<script>
export default {
  data() {
    return {
      obj: {
        hidden: true,
      },
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
  <button @click="this.obj.hidden = false">hide Задание 2</button>
  <button @click="this.obj.hidden = true">hide Задание 3</button>
  <button @click="setDone">{{ obj.hidden ? "show" : "hide" }} Задание 4</button><br />
  <p>&nbsp;&nbsp;&nbsp;&nbsp;</p>
  <p :class="obj">Задание 1</p>
</template>
<style>
p.hidden {
  display: none;
}
</style>
