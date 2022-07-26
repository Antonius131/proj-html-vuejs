<template>
   <header class="container-lg">
      <NavBar />
      <MainJumbotron />
   </header>
</template>

<script>
import NavBar from './NavBar.vue';
import MainJumbotron from './MainJumbotron.vue';

export default {
   components: {
      NavBar,
      MainJumbotron
   }
}
</script>

<style>
   .container-lg {
      padding: 1rem 0rem 1rem 4rem;
   }
</style>