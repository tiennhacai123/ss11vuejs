<template>
  <p>Children File</p>
</template>

<script setup>
import { onBeforeMount, onBeforeUnmount, onUnmounted } from "vue";
onBeforeUnmount(() => {
  console.log("Component is about to be unmounted");
});
onUnmounted(() => {
  console.log("Component has been unmounted");
});
</script>

<style></style>
