<template>
<div class="input-container">
    <label>{{label}}</label>
    <input :type="typeInput" :placeholder="placeHolder" />
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
    align-items: flex-start;
    display: flex;
    flex-direction: column;
    
}

label{
    color: var(--black);
    font-family: 'Quicksand', sans-serif;
    font-size: var(--sm);
    font-weight: 700;
    margin-bottom: 6px;
    
}
input[type="text"],
input[type="password"] {
  background-color: var(--text-input-field);
  border-radius: 10px;
  border:none;
  color: var(--text-input);
  height: 42px;
  margin-bottom: 24px;
  max-width: 480px;
  width: 100%;
}

</style>
