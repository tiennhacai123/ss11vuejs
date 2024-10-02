<template>
  <div>
    <p>Age: {{props.ageChild}}</p>
  </div>
</template>

<script setup>
import { defineProps, onBeforeUpdate, onUpdated } from 'vue'
const props = defineProps(["ageChild"])
console.log(props);

onBeforeUpdate(()=>{
    alert("Gia tri age thay doi")
})
onUpdated(()=>{
})
</script>

<style>

</style>