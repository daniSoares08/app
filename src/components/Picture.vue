<template>
  <div>
    <img :src="avatar" v-bind:alt="descricao">
  </div>
</template>

<script>
  export default {
    name: 'PictureS',
    data() {
      return {
        avatar: 'https://www.google.com.br/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png',
        descricao: 'Logo do Google'
      }
    }
  };
</script>