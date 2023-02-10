<script>
export default {
  data() {
    return {
      items: [1, 2, 3],
    }
  },
  methods: {

    }
}
</script>
<template>
  	<template v-for="elem in items">
		<p>&nbsp;{{ elem }}&nbsp;</p>
		<hr>
    </template>
    <ul v-for="elem in items">
      <li>
        <p>&nbsp;{{ elem }}&nbsp;</p>
      </li>
      <hr>
    </ul>
</template>
