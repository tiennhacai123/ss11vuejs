<template>
  <div>
    <h2>B4</h2>
    <Exercise03Children :ageChild = "age"></Exercise03Children>
    <button @click="increase">Increase age</button>
  </div>
</template>

<script setup>
import Exercise03Children from './Exercise04Children.vue'
import {ref} from 'vue'
    const age = ref(0)
    const increase = ()=>{
        return age.value++;
    }
</script>

<style>

</style>