<script setup>
  import PrimeiroComponent from './components/EntendendoRef.vue';
  import Produtos from './components/Produtos.vue';
  import ProdutoReativos
   from './components/ProdutoReativos.vue';
   import Contador from './components/Contador.vue';
  import ProdutoReativoNaoPrimitivo from './components/ProdutoReativoNaoPrimitivo.vue';
import Formulario from './components/Formulario.vue';
</script>

<template>
  <div>
    <ProdutoReativos/>
    <PrimeiroComponent/>
    <Produtos/>
    <Contador/>
    <ProdutoReativoNaoPrimitivo/>
    <Formulario/>
  </div>
</template>

<style scoped>

</style>
