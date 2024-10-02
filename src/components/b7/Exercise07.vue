<template>
  <div>
    <h2>B7</h2>
    <input type="text" v-model="inputValue" />
  </div>
</template>

<script setup>
import { ref, watch } from "vue";
const inputValue = ref("");
watch(inputValue,(newValue)=>{
    console.log(newValue);
    document.title = newValue;
})
</script>

<style></style>
