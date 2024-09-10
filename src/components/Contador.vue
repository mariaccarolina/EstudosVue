<template>
    <h1>Contador</h1>
    <h3>{{ numero }}</h3>
    <button v-on:click="aumentar">+</button>
    <button v-on:click="diminuir">-</button>
</template>

<script setup>
import { ref } from 'vue';

    const numero = ref(0)
    
    function aumentar() {
        numero.value ++
    }

    function diminuir(){
       if(numero.value > 0){
            numero.value --;
       }
    }
</script>