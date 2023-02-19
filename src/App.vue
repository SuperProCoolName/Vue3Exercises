<script>
export default {
  data() {
    return {
      newItem: "",
      items: ["a", "b", "c", "d", "e"],
    };
  },
  methods: {
    addItemEnd: function () {
      this.items.push(this.newItem);
    },
    addItemBegin: function () {
      this.items.unshift(this.newItem);
    },
  },
};
</script>
<template>
  <input v-model="newItem" />
  <button @click="addItemEnd">add to the end</button>
  <button @click="addItemBegin">add to the beginning</button>
  <ul v-for="(item, index) in items" :key="index">
    <li>
      {{ item }}
    </li>
  </ul>
</template>
