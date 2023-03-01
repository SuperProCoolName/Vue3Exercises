<script>
import Employee from "./components/Employee.vue";
export default {
  components: {
    Employee,
  },
  data() {},
  methods: {
    alo: function () {
      alert("xxx");
    },
    cons: function () {
      console.log("xxx");
    },
  },
};
</script>
<template>
  <Employee @show="alo" @write="cons" />
</template>
