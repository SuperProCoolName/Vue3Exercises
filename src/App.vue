<script>
export default {
  data() {
    return {
      text: 'type',
      data: 'if you see this then something went wrong',
    }
  },
  methods: {
    changeToType: function() {
      this.text = 'type';
    },
    changeToWrite: function() {
      this.text = 'write';
    }
  }
}
</script>
<template>
  <h1>This text is written using something i don't know what to {{ text }} here</h1><br>
  <button @click="changeToWrite">Change to "write"</button><br>
  <button @click="changeToType">Change to "type"</button> 
</template>