<template>
  <div>
    <p>(ref) Count {{ count }}</p>
    <p>(recative) User:{{ user.name }}, Age:{{ user.age }}</p>
    <button @click="count++">Inc Count</button>
    <button @click="count--">Dec Count</button>
    <button @click="user.age++">Inc Age</button>
  </div>
</template>

<script setup>
import { ref, reactive } from "vue";
const count = ref(0);
const user = reactive({
  name: "Nipun",
  age: "23",
});
</script>
