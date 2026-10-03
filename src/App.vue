<script setup lang="ts">
import { ref } from "vue";
import ConditionalRendering from "./ConditionalRendering.vue";
import EmitingEvents from "./EmitingEvents.vue";
import Events from "./Events.vue";
import Loop from "./Loop.vue";
import Methods from "./Methods.vue";
import Props from "./Props.vue";
import TemplateSyntax from "./TemplateSyntax.vue";
import VBind from "./VBind.vue";
import VModel from "./VModel.vue";
import LifeCycleHooks from "./LifeCycleHooks.vue";

//
const message = ref("");
function handleNotify(msg: string) {
  message.value = msg;
}
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
  <!--  -->
  <EmitingEvents @notify="handleNotify" />
  <p v-if="message">{{ message }}</p>
  <!--  -->
  <LifeCycleHooks />
</template>

<style scoped></style>
