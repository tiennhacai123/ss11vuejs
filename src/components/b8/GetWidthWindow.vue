<template>
  <div>
    <h2>B8</h2>
    <p>Chiều rộng hiện tại của cửa sổ: {{ windowWidth }}px</p>
  </div>
</template>

<script lang="ts" setup>
import { ref, onMounted, onBeforeUnmount } from 'vue';

const windowWidth = ref(window.innerWidth);

const updateWidth = () => {
  windowWidth.value = window.innerWidth;
};

onMounted(() => {
  window.addEventListener('resize', updateWidth);
});

onBeforeUnmount(() => {
  window.removeEventListener('resize', updateWidth);
});
</script>

<style scoped>
p {
  font-size: 18px;
  font-weight: bold;
}
</style>
