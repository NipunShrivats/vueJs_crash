<template>
  <div>
    <label>Email:</label>
    <input type="email" placeholder="Enter your Email" v-model="email" />
    <p>Your email is {{ email }}</p>
  </div>
</template>

<script setup>
import { ref } from "vue";
const email = ref("");
</script>
