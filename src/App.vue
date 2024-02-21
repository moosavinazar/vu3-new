<template>
  <h2 @click="increment">{{ count }}</h2>
  <Home title="Home Page" @increment-event="increment"/>
</template>

<script setup>
  import { ref } from 'vue';
  import Home from './components/Home.vue'

  const count = ref(0);
    
  function increment(value) {
    count.value += value;
  }

</script>

<style>

</style>
