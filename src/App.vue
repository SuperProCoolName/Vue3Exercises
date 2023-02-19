<script>
export default {
  data() {
    return {
      var_1: "Задание 1",
      isCtrlPressed: false,
      var_2: "you pressed control + link",
    };
  },
  methods: {
    lag: function () {
      this.var_1 = this.$refs.textField.value;
    },
    leg: function (event) {
      if (event.ctrlKey) {
        this.isCtrlPressed = true;
      }
    },
    handleLeftClick: function (event) {
      if (!event.ctrlKey) {
        this.var_2 = "left";
      }
    },
    handleRightClick: function (event) {
      if (!event.ctrlKey) {
        this.var_2 = "right";
      }
    },
    handleMiddleClick: function (event) {
      if (!event.ctrlKey) {
        this.var_2 = "middle";
      }
    },
  },
};
</script>
<template>
  <input type="text" @keyup.enter="lag" ref="textField" />
  &nbsp;
  <p>{{ var_1 }}</p>
  &nbsp;
  <a
    href="https://www.youtube.com/watch?v=R05dgTwTN6I"
    @click="leg"
    @click.left="handleLeftClick"
    @click.right="handleRightClick"
    @click.middle="handleMiddleClick"
    target="_blank"
    >Задание 2 и 3</a
  >
  &nbsp;
  <p v-if="isCtrlPressed">{{ var_2 }}</p>
</template>
