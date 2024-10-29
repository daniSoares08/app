<template>
  <div>
    <h2>Descrição</h2>
    <InfoIn /> 
    <FormImp />
  </div>
</template>

<script>
  import InfoIn from './Info.vue';
  import FormImp from './form/Form.vue';

  export default {
    name: 'NomePessoa',
    components: {
      InfoIn,
      FormImp,
    },
  };
</script>