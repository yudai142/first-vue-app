<script setup>
import { reactive } from 'vue';

const form = reactive({
  message: 'Hello World',
});

const clickButton = () => {
  console.log(form.message);
};
</script>

<template>
  <h1>Vue 3 入門</h1>
  <p>{{ form.message }}</p>
  <input v-model="form.message" />
  <div><button @click="clickButton">Click</button></div>
</template>