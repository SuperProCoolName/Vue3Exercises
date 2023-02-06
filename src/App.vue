<script>
export default {
  data() {
    return {
      date: 'if you see this then something went wrong'
    }
  },
  methods: {
	show: function() {
    const current = new Date(); 
    const dayOfWeekNumber = current.getDay();
    let dayOfWeek;
    switch (dayOfWeekNumber) {
      case 0:
        dayOfWeek = "Sunday";
        break; 
      case 1:
        dayOfWeek = "Monday";
        break;
      case 2:
        dayOfWeek = "Tuesday";
        break;
      case 3:
        dayOfWeek = "Wednesday";
        break;
      case 4:
        dayOfWeek = "Thursday";
        break;
      case 5:
        dayOfWeek = "Friday";
        break;
      case 6:
        dayOfWeek = "Saturday";
        break;
      default:
        dayOfWeek = "Something went wrong"
        break;
    }
		alert(`Day of week by number = ${dayOfWeekNumber}. Day of week = ${dayOfWeek}`);
	}
}
}
</script>
<template>
  {{ show() }}
</template>