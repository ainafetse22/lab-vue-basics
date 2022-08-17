<template>
  <div>
    <footer>{{msg}}</footer>
  </div>
</template>

<script>
import { ref } from 'vue';

export default {
  setup() { // needed when the component is no SFC
    const msg = ref('Footer Msg');
    return { msg }; // combined with setup()
  },
};

</script>

<style>

</style>
