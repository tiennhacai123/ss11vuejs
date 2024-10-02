<template>
  <div>
    <h2>B2</h2>
    <p>{{count}}</p>
    <button @click="increase">Couter</button>
  </div>
</template>

<script setup>
    import { ref, onBeforeUpdate, onUpdated } from 'vue'
    const count = ref(0)
    onBeforeUpdate(()=>{
         console.log("Dữ liệu đã thay đổi");
    })
    const increase=()=>{
            return count.value++;
        } 
</script>

<style>

</style>