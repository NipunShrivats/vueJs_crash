<template>
  <div>
    <p v-if="status === `loggedIn`">Welcome Back, Ramu</p>
    <p v-else-if="status === `loading`">Checking your credentials...</p>
    <p v-else="status === `loggedOut`">Hi continue to login</p>
  </div>
</template>

<script setup>
import { ref } from "vue";
// const status = ref("loggedIn");
// const status = ref("loading");
const status = ref("loggedOut");
</script>
