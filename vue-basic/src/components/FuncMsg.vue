<template>
<h1>{{showMsg}}</h1>
<p v-show="boolShow">This p is static but shows with V-IF</p>
<img v-if="boolShow" class="img-logo" src="../assets/logo.png" alt="logo">
<button @click="changeShow">ShowSelector</button>
<slot></slot>
</template>

<script setup> // exposed everything to the template, no return needed for var and functions
import { ref, onMounted } from 'vue';

const showMsg = ref('initial message');
const boolShow = ref(true);

const changeShow = () => {
  console.log(boolShow);
  boolShow.value = !boolShow.value;
};

onMounted(() => {
  showMsg.value = ref('Hello from mounted function'); // <div>
});

</script>
<style>
.img-logo{
  filter: grayscale(100%);
}
</style>
