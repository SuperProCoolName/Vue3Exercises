<script>
export default {
  data() {
    return {
      languages: [],
    };
  },
  methods: {},
};
</script>
<template>
  <input type="checkbox" v-model="languages" value="english" />
  &nbsp;
  <p>English</p>
  &nbsp;
  <input type="checkbox" v-model="languages" value="russian" />
  &nbsp;
  <p>Russian</p>
  <input type="checkbox" v-model="languages" value="javascript" />
  &nbsp;
  <p>JavaScript</p>
  &nbsp;
  <ul v-for="elem in languages">
    <li>{{ elem }}</li>
  </ul>
</template>
