<template>
  <div>
    <h2>B3</h2>
    <p>Current Company: {{ company }}</p>
    <p>Age: {{ age }}</p>
    <button @click="randomNum">Random</button>
  </div>
</template>

<script setup>
import { ref } from "vue";
const age = ref(0);
const company = ref("Rikkei Academy");

const randomNum = () => {
  age.value = Math.ceil(Math.random() * 10);
  const randomIndex = Math.floor(Math.random() * companies.value.length);
  company.value = companies.value[randomIndex];
};
const companies = ref(["Rikkei Academy", "Rikkei Education", "Rikkei Fukuoka"]);
</script>

<style></style>
