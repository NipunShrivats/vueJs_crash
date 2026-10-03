<script setup>
import { ref } from "vue";

const tooltipText = ref("click to submit your response.");
</script>
<template>
  <button :title="tooltipText">Submit</button>
</template>
