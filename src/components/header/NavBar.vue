<template>
   <nav>
      <div id="nav-brand">
         <img src="" alt="MaxCoach logo">
      </div>
      <NavMenu />
      <div class="nav-options">
         <NavLang />
         <div id="user-account">
            <i>icon</i>
         </div>
         <div id="user-search">
            <input type="search" placeholder="Search...">
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
      height: 100%;
      padding-left: 4rem;

      .nav-options {
         @include flex-between;

         #user-account,
         .nav-lang {
            padding: 0 .75rem;
         }

         #user-search {
            border-left: 1px solid $bg_primary;
            padding: 1rem;

            input {
               font-size: $nav_items;
               padding: 0.5rem;
               background-color: transparent;
               border: none;
            }
         }
      }
   }

   
</style>