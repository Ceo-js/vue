

<script lang="ts">
   /* 1- importat o componente filho dentro do pai */
   import ComponenteFilho from "./componentes/ComponenteFilho.vue";
   export default {
      /* 2- registrar o componente filho */
      components: {
         ComponenteFilho
      },
      /* definindo props para o componente pai */
      props: {
         cidade: Object,
         nome: String,
         numero: Number,
         lista: Array,
      },
      data() {
         /* ... */
      }
   }
</script>

<template>
   <!-- 3- usar o componente filho -->
   <ComponenteFilho
      props="..."
   />
</template>

<style scoped>
   
</style>