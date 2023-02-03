<script>
export default {
  data() {

  },
  methods: {
    show: function() {
      const current = new Date();
      const date = `${current.getDate()}/${current.getMonth()+1}/${current.getFullYear()}`;
      alert(date);
    }
  }
}
</script>
<template>
  {{ show() }}
</template>