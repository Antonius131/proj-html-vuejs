<template>
   <header class="container-lg">
      <NavBar />
   </header>
</template>

<script>
import NavBar from './NavBar.vue';

export default {
   components: {
    NavBar
   }
}
</script>

<style>
   .container-lg {
      padding: 1rem 0rem 1rem 4rem;
   }
</style>