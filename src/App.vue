<script>
export default {
  data() {
    return {
      choice: "",
      english: true,
      russian: false,
      binary: false,
    };
  },
  methods: {
    eng: function () {
      this.english = true;
      this.russian = false;
      this.binary = false;
    },
    rus: function () {
      this.english = false;
      this.russian = true;
      this.binary = false;
    },
    bin: function () {
      this.english = false;
      this.russian = false;
      this.binary = true;
    },
  },
};
</script>
<template>
  <p v-if="english">What is your mother tongue?</p>
  <p v-if="russian">Какой ваш родной язык?</p>
  <p v-if="binary">
    01110111 01101000 01100001 01110100 00100000 01101001 01110011 00100000
    01111001 01101111 01110101 01110010 00100000 01101101 01101111 01110100
    01101000 01100101 01110010 00100000 01110100 01101111 01101110 01100111
    01110101 01100101 00111111
  </p>
  &nbsp;
  <input
    name="radio"
    type="radio"
    v-model="choice"
    value="English"
    @click="eng"
  />
  &nbsp;
  <input
    name="radio"
    type="radio"
    v-model="choice"
    value="Русский"
    @click="rus"
  />
  &nbsp;
  <input
    name="radio"
    type="radio"
    v-model="choice"
    value="01100010 01101001 01101110 01100001 01110010 01111001"
    @click="bin"
  />
  &nbsp;
  <p>{{ choice }}</p>
</template>
