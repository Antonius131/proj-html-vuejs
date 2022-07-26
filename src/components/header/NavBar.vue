<template>
   <nav>
      <div id="nav-brand">
         <img src="" alt="MaxCoach logo">
      </div>
      <NavMenu />
      <div class="nav-options">
         <div id="nav-lang">
            <select>
               <option value="en" selected>
                  <img src="" alt="en-flag">
                  <p>English</p>
               </option>
               <option value="de">
                  <img src="" alt="de-flag">
                  <p>German</p>
               </option>
               <option value="fr">
                  <img src="" alt="fr-flag">
                  <p>French</p>
               </option>
            </select>
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

export default {
   components: { 
      NavMenu
   }
}
</script>

<style lang="scss">
   @import '../../assets/css/mixins.scss';
   @import '../../assets/css/variables.scss';

   nav {
      @include flex-between;

      #nav-brand {
      }

      .nav-options {
         @include flex-between;

         div {
            padding: 0 .5rem;
         }
      }
   }

   
</style>