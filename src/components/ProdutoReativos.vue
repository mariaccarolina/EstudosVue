<!-- reatividade de valores primitivos -->
 <template>
    <div>
        <h1>Componente Produtos reativos</h1>
        <p>Nome: {{ nome }} | Idade: {{ idade }}</p>
        <!-- o v-on:click="" é usado para ouvir eventos -->
        <button v-on:click="fazerAniversario">Fazer Aniversário</button>
    </div>
 </template>

<!-- escrita mais simplificada: -->
 <!-- sem export defaut -->
  <!-- reatividade -->
 <script setup>
//   ref é uma função que cria reatividade
// para acessar o valor precisamos encapsular no ref e usar o .value para modificar ou acessar o valor da variavel
import { ref } from 'vue';

    const nome = ref("Carol")
    const idade = ref(30)
   
   function fazerAniversario(){
    idade.value ++
   }
</script>