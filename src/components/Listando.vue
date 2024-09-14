<script setup>
import { reactive, ref } from 'vue';

// const quantidade = ref(0);

const produtos = reactive([
    {
        nome: "Fatia Bolo do Amor",
        preco: "R$: 14,00",
        foto: "https://pubimg.band.uol.com.br/files/fbdcbc41b97cb83dbbc0.png",
        quantidade: 0
    },
    {
        nome: "Beijinho do Sol",
        preco: "R$: 10,00",
        foto: "https://s2-receitas.glbimg.com/a_j3JJfSuN3SEw8rrP7rkNg28-w=/0x0:289x249/984x0/smart/filters:strip_icc()/s.glbimg.com/po/rc/media/2012/06/13/15/26/31/815/NL_12523_39933.5426851852.jpg",
        quantidade: 0
    },
    {
        nome: "Torta Mousse Maracujá",
        preco: "R$: 15,00",
        foto: "https://www.receiteria.com.br/wp-content/uploads/torta-mousse-de-maracuja-facil-09-730x548.jpg",
        quantidade: 0
    }
]);

const add = (produto) => {
    produto.quantidade ++;
    console.log("oiii")
}

const remove = (produto) => {
    produto.quantidade --;
    console.log("removendo")
}
</script>

<template>
    <section>
<div v-for="(produto, index) in produtos" :key="index">
    <img v-bind:src="produto.foto" alt="">
    <h3>{{ produto.nome }}</h3>
    <h4>{{ produto.preco }}</h4>
    <div class="caixa">
        <button @click="add(produto)">+</button>
        <button @click="remove(produto)">-</button>
    </div>
    <h2 v-if="produto.quantidade > 0">{{ produto.quantidade }}</h2>
</div>
</section>
</template>

<style scoped>
section{
    display: flex;
}

div{
    background-color: darkred;
    margin: 10px;
    color: wheat;
   text-align: center;
}
img{
    width: 20vw;
    height: 30vh;

}
</style>