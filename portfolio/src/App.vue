<template>
  <div id="app">
    <HomePage />
  </div>
</template>

<script>

import HomePage from "./components/HomePage.vue";

export default {
  name: 'App',
  components: {
    HomePage
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 0 auto;
  background-color: #011126;
}
body{
  background: #011126;
}
</style>
