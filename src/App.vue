<script>
export default {
  data() {
    return {
      task: "Задание",
      task_number: 1,
    };
  },
  methods: {},
};
</script>
<template>
  <input type="text" v-model="task" />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <p>{{ task }}</p>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <p>{{ task.toUpperCase() }}</p>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <input type="number" v-model="task_number" />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <p>{{ task_number ** 2 }}</p>
</template>
