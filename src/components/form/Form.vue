<template>
  <div>
    <form action="" @submit="enviarformulario($event)">
    <div>
      <input type="text" v-model="name">
    </div>
    <div>
      <input type="text" v-model="email">
    </div>
    <InputText />
    <SubmitForm />
    <p>Conteudo</p>
    <p>Conteudo</p>
    <p>Conteudo</p>
    
  </form>
  </div>
  
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
    data() {
      return {
        name: 'Daniel',
        email: 'Daniel@email.com'
      }
    },
    methods: {
      enviarformulario(e) {
        e.preventDefault();

        const name = this.name;
        const email = this.email;

        console.log(name, email);

        // Ajax
        // Inserir no banco de dados

      }
    }
  };
</script>

<style scoped>
 p {
  margin: 150px;
 }
</style>