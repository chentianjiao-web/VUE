<script setup>
import Aside from './components/Aside.vue'
import A3 from './components/A3.vue'
import A2 from './components/A2.vue'
</script>

<template>
  <div class="main">
    <Aside></Aside>
    <A3></A3>
    <A2></A2>
   
  </div>
</template>

<style scoped>
.main{
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: space-between;
}
</style>