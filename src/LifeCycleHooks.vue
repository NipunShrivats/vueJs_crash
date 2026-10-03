<template>
  <div>
    <h2>Dashboard</h2>
    <p v-if="loading">Loading Data...</p>
    <p v-else>{{ data }}</p>
  </div>
</template>

<script setup>
import { ref, onMounted } from "vue";
const data = ref("");
const loading = ref(true);

onMounted(async () => {
  await new Promise((resolve) => setTimeout(resolve, 1500));
  data.value = "Welcome Bitch!";
  loading.value = false;
});
</script>
