<script>
export default {
  data() {
    return {
      visibility_p1: false,
      visibility_p2: false,
      visibility_p3: false,
    }
  },
  methods: {
      toggle_p1: function() {
        this.visibility_p1 = !this.visibility_p1;
      },
      toggle_p2: function() {
        this.visibility_p2 = !this.visibility_p2;
      },
      toggle_p3: function() {
        this.visibility_p3 = !this.visibility_p3;
      },
  }
}
</script>
<template>
  <button @click="toggle_p1">{{ visibility_p1 ? 'hide' : 'show' }}</button><br>
  <p v-if="visibility_p1">text p1</p>
  <button @click="toggle_p2">{{ visibility_p2 ? 'hide' : 'show' }}</button><br>
  <p v-if="visibility_p2">text p2</p>
  <button @click="toggle_p3">{{ visibility_p3 ? 'hide' : 'show' }}</button><br>
  <p v-if="visibility_p3">text p3</p>
  
</template>