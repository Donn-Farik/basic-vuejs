<template>
  <div v-for="el in data" :key="el">
    {{ el.title }}
  </div>
</template>

<script setup>
import { ref } from "vue";
const data = ref([
  {
    title: "CIO",
    description: "Lorem ipsum dolor",
    content: "Lorem ipsum dolor",
  },
  {
    title: "Engineer",
    description: "Lorem ipsum dolor",
    content: "Lorem ipsum dolor",
  },
  {
    title: " developper",
    description: "Lorem ipsum dolor",
    content: "Lorem ipsum dolor",
  },
]);
</script>

<style scooped></style>
