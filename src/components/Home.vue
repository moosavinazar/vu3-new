<template>
  <h2>{{ props.title }}</h2>
  <!-- <button @click="$emit('incrementEvent', 3)">increment</button> -->
  <button @click="sumevent">increment</button>
</template>

<script setup>

    import { defineProps, defineEmits } from 'vue';

    const props = defineProps(['title']);
    const emit = defineEmits(['incrementEvent']);

    function sumevent() {
        emit('incrementEvent', 3);
    }

</script>

<style>

</style>