<script setup>
import { ref } from 'vue';
const contador = ref(0)
const valor = ref(true);
</script>

<template>
    <h1>Contador carrinho</h1>
    <button @click="contador ++">Clique para adicionar</button>
    <button @click="contador --" v-if="contador > 0">Clique para adicionar</button>
    <h3>{{ contador }}</h3>

    <!-- <button @click="valor = !valor">Trocar de estilo</button>
            {{valor }}
     <p :class="{trocar: !valor}"  >Eu vou trocar de estilo</p> -->
    <button @click="valor = !valor">Mude a cor:</button>
    <p :class="{trocar: !valor}">Olá! Irei trocar!</p>*

</template>

<style scoped>
p{
    background-color: rgb(195, 13, 147);
     border: none;
    padding: 10px 20px;
    border-radius: 20px;
    font-size: 20px;
    color: white;
    cursor: pointer;
}
.trocar{
    background-color: red;
    border: none;
    padding: 10px 20px;
    border-radius: 20px;
    font-size: 20px;
    color: white;
    cursor: pointer;
}
</style>