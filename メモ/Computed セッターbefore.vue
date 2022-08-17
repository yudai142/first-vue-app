<script setup>
import { reactive, computed } from 'vue';

const user = reactive({
  firstName: 'John',
  lastName: 'Doe',
});

const fullName = computed(() => `${user.firstName} ${user.lastName}`);

const changeName = () => {
  fullName.value = 'Jane Doe';
};
</script>

<template>
  <h1>Vue 3 入門</h1>
  <h2>fullName: {{ fullName }}</h2>
  <button @click="changeName">Change Name</button>
</template>