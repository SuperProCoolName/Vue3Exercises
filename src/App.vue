<script>
export default {
  data() {
    return {
      arr: ['x', 'y', 'z'],
      array: [1, 2, 3],
    }
  }
}
</script>
<template>
  <p>№1: arr[0]: {{ arr[0] }}</p><br>
  <p>arr[1]: {{ arr[1] }}</p><br>
  <p>arr[2]: {{ arr[2] }}</p><br>
  <p>№2: array[0] + array[1] + array[2] = {{ array[0] + array[1] + array[2] }}</p>
</template>