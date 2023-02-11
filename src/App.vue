<script>
export default {
  data() {
    return {
      hrefs: [
        {href: '1.html', text: 'text1'},
        {href: '2.html', text: 'text2'},
        {href: '3.html', text: 'text3'},
		  ],
      products: [
        {
          name: 'product1',
          price: 100,
          quantity: 5
        },
        {
          name: 'product2',
          price: 200,
          quantity: 4
        },
        {
          name: 'product3',
          price: 300,
          quantity: 3
        },
		  ]
    }
  },
  methods: {

    }
}
</script>
<template>
  Задание 1&nbsp;|&nbsp;
  <ul v-for="smh in hrefs">
    <li><a href="{{ smh.href }}">{{ smh.text }}</a></li>
  </ul>
  <br>Задание 2&nbsp;|&nbsp;
  <table v-for="product in products">
    <tr>
      <td>{{ product.name }}</td>
      <td>{{ product.price }}</td>
      <td>{{ product.quantity }}</td>
    </tr>
  </table>
</template>
<style>
  table {
    display: flex;
    justify-content: flex-start;
    flex-direction: column-reverse;
  }
</style>