<template>
<H1>{{showMsg}}</H1>
</template>

<script setup> // exposed everything to the template, no return needed for var and functions
import { ref, onMounted } from 'vue';

const showMsg = ref('initial message');
onMounted(() => {
  showMsg.value = ref('Hello from mounted function'); // <div>
});

</script>
<style>

</style>
