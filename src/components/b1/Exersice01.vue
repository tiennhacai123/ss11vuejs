<template>
  <div>
    <h2>B1</h2>
    <p>in thông báo ra màn hình console với nội dung “Component mounted” khi component được mount vào trong DOM</p>
    
  </div>
</template>

<script setup>
    import {onBeforeMount, onMounted} from 'vue'
    onBeforeMount(()=>{
        console.log("onBeforeMount duoc goi");
        console.log("Component mounted");
        
    })
    onMounted(()=>{
        console.log("onMounted duoc goi");
        
    })
</script>

<style>

</style>