<template>
<div class="input-container">
  <div class="input-wrapper">
    <label>{{label}}</label>
    <input :type="typeInput" :placeholder="placeHolder" />
  </div>
</div>
</template>

<script>
import "../style/theme.css";
export default {
  name: "Input",
  props: {
    label: String,
    typeInput: {
        default: 'text',
        type: String,
    },
    placeHolder: {
        default: 'Fill the field',
        type: String,
    }
    
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.input-container{
    
  display: flex;
  flex-direction: column;
  width: 100%;
  align-content: center;
  
}

.input-wrapper{
  display:flex;
  flex-direction: column;
  width:320px;
  align-self: center;
}

label{
    color: var(--black);
    font-family: 'Quicksand', sans-serif;
    font-size: var(--sm);
    font-weight: 700;
    margin-bottom: 6px;
    align-self: flex-start;
    

    
}
input[type="text"],
input[type="password"] {
  background-color: var(--text-input-field);
  border-radius: 10px;
  border:none;
  color: var(--text-input);
  height: 42px;
  margin-bottom: 24px;
  max-width: 320px;
  width: 100%;
  align-self: center;
  
}

</style>
