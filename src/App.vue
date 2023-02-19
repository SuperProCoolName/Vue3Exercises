<script>
export default {
  data() {
    return {
      selected: "Выберите город",
    };
  },
  methods: {},
};
</script>
<template>
  <select v-model="selected">
    <option>Амстердам</option>
    <option>Лондон</option>
    <option>Нью-Йорк</option>
    <option>Токио</option>
    <option>Новокузнецк</option>
    <option>Париж</option>
  </select>
  &nbsp;
  <p>{{ selected }}</p>
</template>
