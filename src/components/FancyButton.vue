<template>
  <button> 
    <slot name="icon">➡️</slot>
    <slot>Submit</slot>
  </button>
</template>
  
  <style scoped>
  .content{
  text-align: center;
}
button{
  width: 12rem;
  margin: 30px auto;
  font-size: 2rem;
}
  </style>

  <script setup>

  </script>
  