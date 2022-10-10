<script setup>
import Home from "./components/Home.vue";
import Header from "./components/Header.vue";
</script>

<template>
  <header><Header /></header>

  <main>
    <Home />
  </main>
  
  <footer>©Monica M Nikolaisen 2022</footer>
</template>

<style>
footer{
margin-top:2em;
text-align:center;
}
</style>
