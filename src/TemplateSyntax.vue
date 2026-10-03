<script setup>
import { template } from "vue";
import { ref } from "vue";
const userName = ref("Rawat Nipun");
const Notification = ref(7);
</script>
;
<template>
  <div>
    <h2>Welcome back, {{ userName }}!</h2>
    <p>Notifications: {{ Notification }}</p>
  </div>
</template>
;
