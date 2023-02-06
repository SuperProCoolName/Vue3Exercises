<script>
export default {
  data() {
    return {
      date: 'if you see this then something went wrong'
    }
  },
  methods: {
	show: function() {
    const number = this.$refs.inputField.value;
		alert(`${number * number}`);
	},
  power_two: function() {
    alert(`${2 * 2}`);
  },
  power_three: function() {
    alert(`${3 * 3}`);  
  }
}
}
</script>
<template>
  <h3>Enter number:</h3>
  <input type="number" ref="inputField"><br>
  <button @click="show()">Try it</button>

  <button @click="power_two()">Two to the power of 2</button><br>
  <button @click="power_three()">Three to the power of 2</button>
</template>