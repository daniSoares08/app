<template>
  <ul>
    <li> <a href="#">Home</a></li>
    <li> <a href="#">Projetos</a></li>
    <li> <a href="#">contato</a></li>
  </ul>
</template>

<script>
  export default {
    name: 'HeaderOne',
    data() {
      return {
        title: 'Welcome to Vue.js'
      }
    }
  }
</script>


<!-- scoped define que o estilo é apenas para esse elemento -->
<style scoped>
  ul {
    display: flex;
    justify-content: space-around;
    justify-items:auto;
    list-style: none;
    padding: 0;
    text-align: center;

  }
  li {
    color: aqua;
    display: flex;
    justify-content: center;
    padding: 10;
    text-align: center;
  }
  a {
    color: rgb(255, 0, 0);
    text-decoration: none;
    transition: .5s;
  }
</style>