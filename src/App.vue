<script setup>
import navbarVue from "./components/navbar.vue";
import footerVue from "./components/footer.vue";
import postsVue from "./components/posts.vue";
import { ref } from "vue";
const isTrue = ref(true);
const changeColor = () => {
  return (document.querySelector("#patata").style.backgroundColor = "red");
};
</script>

<template>
  <!-- iteration 1 -->
  <navbarVue />
  <br />
  <footerVue />
  <br />
  <postsVue />
  <br />
  <!-- iteration 2 -->
  <div>
    {{ 2 + 2 }}
  </div>
  <!-- Iteration 3 -->
  <p v-if="isTrue">show me please</p>
  <br />
  <!-- Iteration 5 -->
  <div>
    <h1 id="patata">we are the champion</h1>
    <button v-on:click="changeColor">click to change the color</button>
  </div>
</template>

<style scoped></style>
