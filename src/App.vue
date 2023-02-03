<script>
export default {
  data() {
    return {
      text: 'Click me',
      href: 'https://www.youtube.com/watch?v=dQw4w9WgXcQ', // видео 
    }
  }
}
</script>
<template>
  <a :href=href>{{ text }}</a>
</template>