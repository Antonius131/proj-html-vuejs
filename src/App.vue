<template>
  <div id="app">
    <MainHeader />
    <MainContent />
    <MainFooter />
  </div>
</template>

<script>
import MainHeader from './components/header/MainHeader.vue';
import MainContent from './components/main/MainContent.vue';
import MainFooter from './components/footer/MainFooter.vue';
import '/node_modules/bootstrap/dist/js/bootstrap.min.js';

export default {
  name: 'App',
  components: {
    MainHeader,
    MainContent,
    MainFooter
  }
}
</script>

<style lang="scss">
  @import '/node_modules/bootstrap/scss/bootstrap.scss';
  @import './assets/css/variables.scss';
  
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    color: #2c3e50;
  }

  .container {
    width: 70%;

      .row {
        padding: $row_padding;
      }
  }
</style>
