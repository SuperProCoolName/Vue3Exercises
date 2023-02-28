<script>
export default {
  data() {
    return {
      items: ["a", "b", "c", "d", "e"],
    };
  },
  methods: {
    removeItem: function (index) {
      this.items.splice(index, 1);
    },
  },
};
</script>
<template>
  <ul>
    <li v-for="(item, index) in items" :key="index">
      <button @click="removeItem(index)">{{ item }}</button>
    </li>
  </ul>
</template>
