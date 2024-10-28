<script setup>
import LandingPage from './views/LandingPage.vue';
</script>

<template>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400..700&display=swap" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css2?family=Inter+Tight:ital,wght@0,100..900;1,100..900&display=swap" rel="stylesheet">
    
  <div id="app">
    <LandingPage />
  </div>
</template>

<script>
export default {
  name: 'App',
  components: {
    LandingPage,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.inter-tight{
  font-family: "Inter Tight", sans-serif;
  font-optical-sizing: auto;
  font-style: normal;
}
.dancing-script {
  font-family: "Dancing Script", cursive;
  font-optical-sizing: auto;
  font-style: normal;
}
</style>
