<script>
import Employee from "./components/Employee.vue";
export default {
  components: {
    Employee,
  },
  data() {
    return {
      name: "John",
    };
  },
  methods: {
    cons_name: function (name) {
      console.log(name);
    },
    cons_sal: function (name, salary) {
      console.log(name, salary);
    },
  },
};
</script>
<template>
  <input type="text" v-model="name" />
  <Employee @write="cons_name" @show="cons_sal" />
</template>
