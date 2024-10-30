<template>
  <div>
    <p v-if="estaTrabalhando">Estou trabalhando no momento</p>
    <p v-else>Estou procurando novas oportunidades</p>
    <p>Acesse esse portfólio <a v-bind:href="meu_link">clicando aqui</a></p>

    <p>Utilizo as seguintes tecnologias para o backend:</p>
    <ul>
      <li v-for="(tecnologia, index) in backend" :key="index">{{ tecnologia }}</li>
    </ul>

    <p>Utilizo as seguintes tecnologias para o frontend:</p>
    <ul>
      <li v-for="tecnologia in frontend" :key="tecnologia.id">
        {{ tecnologia.lenguage }}
      </li>
    </ul>


    <button @click="showEmail"> {{ textobotao }} </button>
    <p v-if="mostraemail">MEU EMAIL AQUI</p>

  </div>
</template>

<script>
  export default {
    name: 'InfoIn',
    data() {
      return {
        estaTrabalhando: false,
        mostraemail: false,
        meu_link: 'https://meu_link.com',
        textobotao: 'Mostrar email',
        backend: ['JavaScript', 'PHP', 'Python'],
        frontend: [
          {id: 1, lenguage: 'HTML'},
          {id: 2, lenguage: 'CSS'},
          {id: 3, lenguage: 'Vue'},
        ]
      }
    },
    
    methods: {
      showEmail() {
        this.mostraemail = !this.mostraemail
        if(!this.mostraemail){
          this.textobotao = 'Mostrar email'
        } else {
          this.textobotao = 'Esconder email'
        }
        }}
    }
</script>
