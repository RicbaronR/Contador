<script setup>
  import { ref } from 'vue';

  const contador = ref(0)

  function incrementar(){
    contador.value++
  }

  function decrementar(){
    contador.value--
  }
</script>

<template>
  <h1>Contador do Ricardo</h1>
  <p>Valor do Contador: {{ contador }}</p>
  <button v-on:click="incrementar">+</button>
  <button @click="decrementar">-</button>

  <!--POdemos puxar com v-on ou @, só funciona com o v-on-->
</template>

<style scoped>
  button{
    background-color: black;
    color: white;
    border-radius: 20px;
    font-size: 20px;
  }
</style>
