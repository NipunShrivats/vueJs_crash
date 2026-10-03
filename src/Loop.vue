<template>
  <ul>
    <li v-for="(course, index) in courses" :key="index">
      {{ index + 1 }}.{{ course }}
    </li>
  </ul>
  <div></div>
</template>

<script setup>
import { ref } from "vue";

const courses = ref(["Vue", "React", "Angular"]);
</script>
