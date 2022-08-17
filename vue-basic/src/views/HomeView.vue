<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <FuncMsg></FuncMsg>
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>

<script>
import FuncMsg from '@/components/FuncMsg.vue';
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue';

export default {
  name: 'HomeView',
  components: {
    FuncMsg,
  },
};
</script>
