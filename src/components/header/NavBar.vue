<template>
   <nav>
      <div id="nav-brand">
         <img src="" alt="MaxCoach logo">
      </div>
      <NavMenu />
      <div class="nav-options">
         <div id="nav-lang">
            <NavLang />
         </div>
         <div id="user-account">
            <i>icon</i>
         </div>
         <div id="user-search">
            <input type="search" placeholder="Search">
            <button class="btn">icon</button>
         </div>
      </div>
   </nav>
</template>

<script>
import NavMenu from './NavMenu.vue';
import NavLang from './NavLang.vue';

export default {
   components: {
      NavMenu,
      NavLang
   }
}
</script>

<style lang="scss">
   @import '../../assets/css/mixins.scss';
   @import '../../assets/css/variables.scss';

   nav {
      @include flex-between;

      .nav-options {
         @include flex-between;

         div {
            padding: 0 .5rem;
         }
      }
   }

   
</style>