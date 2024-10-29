<template>
  <FirstComponent />
  <LifeCycle />
  <Pessoa />
  <PictureS />
  
</template>

<script>
  import FirstComponent from './components/FirstComponent.vue'
  import LifeCycle from './components/LifeCycle.vue';
  import Pessoa from './components/Pessoa.vue';
  import PictureS from './components/Picture.vue';

  export default {
    name: 'App',
    components: {
      FirstComponent,
      LifeCycle,
      Pessoa,
      PictureS
    }
  }
</script>