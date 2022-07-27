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
  @import '../node_modules/bootstrap/scss/bootstrap.scss';
  @import './assets/css/mixins.scss';
  @import './assets/css/variables.scss';
  
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    color: #2c3e50;
  }

  section {
    padding: $section_padding;
  }

  .container {
    width: 70%;

      .row {
        padding: $row_padding;
      }

      h4 {
        color: $brand_secondary;
        font-weight: 300;
        margin-bottom: 2rem;
      }

      h3 {
        color: $brand_primary;
      }
  }
</style>
