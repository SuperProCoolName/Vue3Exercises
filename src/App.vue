<script>
export default {
  data() {
    return {
      cost: 50,
      amount: 3,
      price: 'Press to compute the price',
    }
  },
  methods: {
    computePrice: function() {
      this.price = (this.cost * this.amount);
    }
  }
}
</script>
<template>
  <h3>Enter number for cost:</h3>
  <input type="number" v-model.number="cost" ref="costField">
  <h3>Enter number for amount:</h3>
  <input type="number" v-model.number="amount" ref="amountField">
  <button @click="computePrice">{{ price }}</button>
</template>