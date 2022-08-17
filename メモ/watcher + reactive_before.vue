<script setup>
import { reactive, watch } from 'vue';

const state = reactive({
  count: 0,
});

watch(state.count, (count, previousCount) => {
  console.log('count:', count);
  console.log('previousCount:', previousCount);
});
</script>

<template>
  <h1>Vue 3 入門</h1>
  <button @click="state.count++">Count:{{ state.count }}</button>
</template>