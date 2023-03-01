<script>
import Employee from "./components/Employee.vue";
export default {
  components: {
    Employee,
  },
  data() {
    return {
      name: "John",
      salary: 300,
      age: 28,
    };
  },
};
</script>
<template>
  <Employee :name="name" :salary="salary" :age="age" />
</template>
