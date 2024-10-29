<template>
  <form action="">
    <InputText />
    <SubmitForm />
  </form>
</template>

<script>
import InputText from './inputText.vue';
import SubmitForm from './Submit.vue';

  export default {
    name: 'FormImp',
    components: {
      InputText,
      SubmitForm,
    },
  };
</script>