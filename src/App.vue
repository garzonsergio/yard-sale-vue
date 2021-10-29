<template>
  <Hero />
  <Hero :color="'#FF0000'" :height="50" />
  <Hero :color="'#0000FF'" />
</template>
// <img alt="Vue logo" src="./assets/logo.png" />


<script>
import Hero from "./components/Hero.vue";

export default {
  name: "App",
  components: {
    Hero,
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
  margin-top: 60px;
}
</style>
