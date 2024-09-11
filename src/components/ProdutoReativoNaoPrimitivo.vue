<script setup>
import { reactive } from 'vue';

const pessoa = reactive({
    nome: "Carol",
    idade: 30
})

function fazerAniversario(){
    pessoa.idade ++
}

function mudarNome(){
    pessoa.nome = "Débora"
}
</script>

<template>
    <h1>reactive</h1>
   <p>A {{ pessoa.nome }} vai fazer {{ pessoa.idade }} anos</p>
   <button @click="fazerAniversario">Mudar idade</button>
   <button @click="mudarNome">Mudar Nome</button>
</template>