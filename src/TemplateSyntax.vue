<template>
  <div>
    <h2>Welcome back, {{ userName }}!</h2>
    <p>Notifications: {{ Notification }}</p>
  </div>
</template>
;

<script setup>
import { template } from "vue";
const userName = ref("Rawat Nipun");
const Notification = ref(7);
</script>
;
