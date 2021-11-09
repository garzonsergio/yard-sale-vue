<template>
<div class="input-container">
  <div class="input-wrapper">
    <label>{{label}}</label>
    <input :type="typeInput" :placeholder="placeHolder" v-model="label1"/>
  </div>
</div>

<p> {{label1}} </p>
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
  data (){
    return {
      label1: '',
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.input-container{
    
  align-content: center;
  display: flex;
  flex-direction: column;
  width: 100%;
  
}

.input-wrapper{
  align-self: center;
  display:flex;
  flex-direction: column;
  width:320px;
}

label{
    align-self: flex-start;
    color: var(--black);
    font-family: 'Quicksand', sans-serif;
    font-size: var(--sm);
    font-weight: 700;
    margin-bottom: 6px;
    

    
}
input[type="text"],
input[type="password"],
input[type="email"]{
  align-self: center;
  background-color: var(--text-input-field);
  border-radius: 10px;
  border:none;
  color: var(--text-input);
  height: 42px;
  margin-bottom: 24px;
  max-width: 320px;
  width: 100%;
  
}

</style>
