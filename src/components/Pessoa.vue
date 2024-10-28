<template>
  <div>
    <h2>Descrição</h2>
    <InfoIn /> <!-- Se é esse o nome do componente mesmo -->
  </div>
</template>

<script>
  import InfoIn from './Info.vue';

  export default {
    name: 'NomePessoa',
    components: {
      InfoIn, // aqui tava faltando vírgula
    },
  };
</script>