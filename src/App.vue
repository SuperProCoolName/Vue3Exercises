<script>
export default {
  data() {

  },
  methods: {
    show: function() {
      const current = new Date();
      const date = `${current.getDate()}/${current.getMonth()+1}/${current.getFullYear()}`;
      alert(date);
    }
  }
}
</script>
<template>
  <p>№1: <button @click="show">text</button></p>
  <p>№1: <button @pointerenter="show">text</button></p>
</template>