<template>
  <Hero :height="43" />
  <Input :label="'Email address'" />
  <Input
    :label="'Password'"
    :typeInput="'password'"
    :placeHolder="'*********'"
  />
  <Button :textButton="'Log in'"/>
  
</template>
 <!-- 
 TODO: Implement this component after set the <Input /> 
 <Form :fields="[{name: 'xname', type: 'text'}, {}]"/> 
 -->

<script>
import Hero from "./components/Hero.vue";
import Input from "./components/Input.vue";
import Button from "./components/Button.vue";

export default {
  name: "App",
  components: {
    Hero,
    Input,
    Button,
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
