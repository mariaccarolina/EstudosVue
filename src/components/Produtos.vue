<template>
    <h1>{{nomeProduto }}</h1>
</template>


<script setup>
const nomeProduto = "Livro"
const codigoProduto = 12345
//função setup como propriedade, não precisamos do
//  return

</script>
<!-- <script>
//temos duas formas de inserir a lógica de uma aplicação
//Options API - É  a forma mais antiga e tradicional de um componente vue, usando objetos de opçõescomo data(dados), methods, computed e etc. Dessa forma sendo organizado em sessoes claras, cada uma com uma responsabilidade especifia.
//ex:
// export default {
//     data() {
//         return{
//             nomeProduto:"Caneta",
//             codigoProduto: "12345"
//         }
//     }
// }

// Outra forma de inserir a lógica em uma aplicação vue é a composition API, foi introduzida no Vue3 para proporcionar mais flexibilidade e reutilização de código, ela permite que você use funções como ref, reactive, e computed para definir a reatividade, lógica e outras funcionalidades de componentes de forma mais granular e modular ex:

export default {
    setup() {
        const nomeProduto = "Caneta"
        const codigoProduto = 12345
        return {nomeProduto, codigoProduto}
    }
}

</script> -->