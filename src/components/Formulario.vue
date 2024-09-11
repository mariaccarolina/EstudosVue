<template>
    <h1>Formulário com o two-way data binding</h1>
    <input
     type="text"
      v-bind:value="valor"
       @input="(e)=>valor = e.target.value">
    <!-- evento d input,  uma função que ta recebendo como paramentro o evento(e)  quando digitar, iremos jogar na variavel-->
    <p> Estou digitando: {{ valor }}</p>
</template>

<script setup>
import { ref } from 'vue';

const valor = ref("Vue é uma maravilha!")
console.log(valor)
</script>