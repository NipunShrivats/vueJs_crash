<template>
  <div>
    <h2>Name:{{ name }}</h2>
    <h2>Email:{{ email }}</h2>
  </div>
</template>

<script setup>
defineProps({
  name: String,
  email: String,
});
</script>
