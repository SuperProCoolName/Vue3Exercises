<script>
export default {
  data() {
    return {
      data: {
      user1: '100$',
      user2: '200$',
      user3: '300$',
      }
    }
  },
  methods: {

    }
}
</script>
<template>
  <ul>
    Задание 1
    <li v-for="value in data">{{ value }}</li>
  </ul>
  <ul>
    Задание 2
    <li v-for="(value, key) in data">{{ key }} - {{ value }}</li>
  </ul>
  <ul>
    Задание 3
    <li v-for="(value, key, index) in data">{{ key }} - {{ value }} - {{ index }}</li>
  </ul>
  <ul>
    Задание 4
    <li v-for="(value, key, index) in data">{{ key }} - {{ value }} - {{ index + 1 }}</li>
  </ul>
</template>
