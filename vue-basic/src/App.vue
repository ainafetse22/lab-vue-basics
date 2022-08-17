<template>
  <div>
    <NavBar></NavBar>
    <router-view></router-view>
    <FooterDiv></FooterDiv>
  </div>
</template>
<script>
import NavBar from '@/components/NavBar.vue';
import FooterDiv from '@/components/FooterDiv.vue';

export default {
  name: 'App',
  components: {
    NavBar,
    FooterDiv,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

</style>
