<script setup lang="ts">
import ConditionalRendering from "./ConditionalRendering.vue";
import Events from "./Events.vue";
import Loop from "./Loop.vue";
import Methods from "./Methods.vue";
import Props from "./Props.vue";
import TemplateSyntax from "./TemplateSyntax.vue";
import VBind from "./VBind.vue";
import VModel from "./VModel.vue";
</script>

<template>
  <TemplateSyntax />
  <VBind />
  <VModel />
  <ConditionalRendering />
  <Loop />
  <Methods />
  <Events />
  <Props name="LALA" email="lala.23@gmail.com" />
</template>

<style scoped></style>
