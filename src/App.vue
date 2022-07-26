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
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  color: #2c3e50;
}
</style>
