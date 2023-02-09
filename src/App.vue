<script>
export default {
  data() {
    return {
      age: "if you see this then something went wrong",
    }
  },
  methods: {

  }
}
</script>
<template>
  <h3>Enter age: </h3><br>
  <input type="number" v-model.number="age">
  <p v-if="age < 18">Подросток</p>
  <p v-else-if="age < 25">Молодой человек</p>
  <p v-else-if="age >= 25">Мужчина</p>
</template>