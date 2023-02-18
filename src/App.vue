<script>
export default {
  data() {
    return {
      number: 1,
      number_square: "Задание 1",
      numero_uno: 0,
      numero_dos: 0,
      sum_number: "Задание 2",
      text_uno: "placeholder",
      text_dos: "placeholder",
      fullName: "",
      userName: "",
      userSurname: "",
      userPatronymic: "",
    };
  },
  methods: {
    square: function () {
      this.number_square = this.number ** 2;
    },
    sum: function () {
      this.sum_number = this.numero_uno + this.numero_dos;
    },
    swap: function () {
      const temp = this.text_uno;
      this.text_uno = this.text_dos;
      this.text_dos = temp;
    },
    split: function () {
      this.userSurname = this.fullName.split(" ")[0];
      this.userName = this.fullName.split(" ")[1];
      this.userPatronymic = this.fullName.split(" ")[2];
    },
  },
};
</script>
<template>
  <input type="number" v-model="number" />
  <button @click="square">Square of number</button>
  &nbsp;
  <p>{{ number_square }}</p>
  &nbsp;
  <input type="number" v-model="numero_uno" />
  <input type="number" v-model="numero_dos" />
  <button @click="sum">Sum of numbers</button>
  &nbsp;
  <p>{{ sum_number }}</p>
  &nbsp;
  <input type="text" v-model="text_uno" />
  <input type="text" v-model="text_dos" />
  <button @click="swap">Swap values</button>
  &nbsp;
  <input type="text" v-model="fullName" />
  <button @click="split">Split full name</button>
  <p>Surname = {{ userSurname }}</p>
  <p>Name = {{ userName }}</p>
  <p>Patronymic = {{ userPatronymic }}</p>
</template>
