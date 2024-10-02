<template>
  <div>
    <h2>B6</h2>
    <button @click="increase">Increment</button>
  </div>
</template>

<script setup>
    import {ref} from 'vue'
    const count = ref(0);
    const increase =()=>{
        document.title=count.value++;
    }
    
</script>

<style>

</style>