<template>
  <div>
    <h2>B9</h2>
    <p>Count: {{count}}</p>
  </div>
</template>

<script setup>
    import {ref ,onBeforeMount, onMounted} from 'vue'
    const count = ref(0);
    onMounted(()=>{
        window.setInterval(()=>{
            count.value++
        },1000)
    })
</script>

<style>

</style>