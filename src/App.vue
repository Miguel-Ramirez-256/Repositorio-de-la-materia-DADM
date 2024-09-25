<script setup>
import { ref } from 'vue';
// Modelo
const header = ref('App lista de compras');
const items = ref([
  {id:'0', label: '10 bolillos'},
  {id:'1', label: '1 crema de litro'},
  {id:'2', label: '1/4 de jamon'},
  {id:'3', label: '1 nutella'}
]);
const newItem = ref("");
</script>

<template>
  <h1>
   <i class="material-icons shopping-cart-icon">local_mall</i> 
    {{ header }} 
  </h1>
  <input v-model="newItem" type="text" placeholder="Agregar un articulo"> {{ newItem }} </input>
  <ul>
    <li v-for="item in items" :key="item.id"> 🛍️ {{  item.label }} </li>
  </ul>
</template>

<style scoped>
.shopping-cart-icon{
  font-size: 2rem;
}
</style>
