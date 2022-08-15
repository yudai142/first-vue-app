<script setup>
const count = $ref(0);

const addCount = () => {
  count++;
};
</script>

<template>
  <h1>Vue 3 入門</h1>
  <button type="button" @click="addCount">count is: {{ count }}</button>
</template>