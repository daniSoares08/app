<template>
  <div>
    <p v-if="estaTrabalhando">Estou trabalhando no momento</p>
    <p v-else>Estou procurando novas oportunidades</p>
    <p>Utilizo as seguintes tecnologias:</p>
    <ul>
      <li v-if="4 > 2">JavaScript</li>
      <li>PHP</li>
      <li>Python</li>
    </ul>
    <p>Acesse esse portfólio <a v-bind:href="meu_link">clicando aqui</a></p>
  </div>
</template>

<script>
  export default {
    name: 'InfoIn',
    data() {
      return {
        estaTrabalhando: false,
        meu_link: 'https://meu_link.com'
      }
    }
  };
</script>
