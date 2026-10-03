<template>
  <div>
    <button @click="sendMessage">Click to send</button>
  </div>
</template>

<script setup>
const emit = defineEmits(["notify"]);
function sendMessage() {
  emit("notify", "Hello from child");
}
</script>
