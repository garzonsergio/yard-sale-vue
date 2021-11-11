<template>
  <div class="button-container">
    <button type="button">{{ textButton }}</button>
  </div>
</template>

<script>
import "../style/theme.css";
export default {
  name: 'Button',
  props:{
    textButton: {
      type: String,
    }
  }
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

button{
  background-color: var(--hospital-green);
  border-radius: 10px;
  border: none;
  color: var(--white);
  font-family: 'Quicksand', sans-serif;
  font-size: var(--md);
  height: 60px;
  max-width: 320px;
  width:90%;
}


</style>
