<script>
import Employee from "./components/Employee.vue";
export default {
  components: {
    Employee,
  },
};
</script>
<template>
  <Employee :arg="{ name: 'John', surname: 'Smith', age: 28 }" />
</template>
