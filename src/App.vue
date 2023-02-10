<script>
export default {
  data() {
    return {
      items: [1, 2, 3, 4, 5],
    }
  },
  methods: {

    }
}
</script>
<template>
    <div class="red-box"><div v-for="elem in items">{{ elem }} &nbsp;</div></div>
    <div class="red-box"><br><div v-for="elem in items">{{ elem ** 2 }} &nbsp;</div></div>
    <div class="red-box right"><div v-for="elem in items"><ul><li>{{ elem }}</li></ul>&nbsp;</div></div>
</template>
<style>
div {
  display: flex;
}
.red-box {
  border: 5px solid red;
  margin: 10px;
  padding: 2px;
}
div.right {
  margin-top: 10px;
  display: flex;
  flex-direction: column;
}
</style>
