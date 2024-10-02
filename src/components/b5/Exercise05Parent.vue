<template>
  <div>
    <h2>B5</h2>
    <button @click="show">Toggle</button>
    <Exercise05Children v-if="isshow"></Exercise05Children>
  </div>
</template>

<script setup>
    import Exercise05Children from './Exercise05Children.vue'
    import {ref} from 'vue'
    const isshow = ref(true)
    const show = ()=>{
        isshow.value = !isshow.value
    }
    
</script>

<style>

</style>