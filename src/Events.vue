<template>
  <div>
    <input v-model="name" type="text" placeholder="Enter Your name" />
    <button @click="handleSubmit">Submit</button>
    <p v-if="greeting">{{ greeting }}</p>
  </div>
</template>

<script setup>
import { ref } from "vue";
const name = ref("");
const greeting = ref("");

console.log("name", name);
console.log("greeting", greeting);

function handleSubmit() {
  if (name.value.trim()) {
    greeting.value = `Hello, ${name.value}`;
  } else {
    greeting.value = "Please Enter you name.";
  }
}
</script>
