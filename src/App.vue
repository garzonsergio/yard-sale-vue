<template>
  <Hero :height="43" />
    <Input :label="'Email address'" />
    <Input :label="'Password'" :typeInput="'password'" :placeHolder="'*********'"/>
    <!-- <Form :fields="[{name: 'xname', type: 'text'}, {}]"/> -->
</template>


<script>
import Hero from "./components/Hero.vue";
import Input from "./components/Input.vue";

export default {
  name: "App",
  components: {
    Hero,
    Input,
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
