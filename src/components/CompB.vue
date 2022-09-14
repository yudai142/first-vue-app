<script setup>
  const { message } = defineProps(['message']);
  </script>
  
  <template>
    <h3>CompBコンポーネント</h3>
    <p>{{ message }}</p>
  </template>
