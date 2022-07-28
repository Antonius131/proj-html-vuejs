<template>
   <nav class="navbar navbar-expand-lg">
      <div class="container-fluid">
         <div class="col-2">
            <a class="navbar-brand" href="#">Navbar</a>
         </div>
         <div class="col-10">
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
               <div class="col-8">
                  <div class="col-12">
                     <NavMenu />
                  </div>
               </div>
               <div class="col-4 d-flex nav-user-options">
                  <div class="col-2 flags-box">
                     <img src="" alt="">
                  </div>
                  <div class="col-4">                  
                     <select class="form-select">
                        <option selected>English</option>
                        <option value="1">German</option>
                        <option value="2">French</option>
                     </select>
                  </div>
                  <div class="col-2 icon-box">
                     <i class="fa-solid fa-circle-user"></i>
                  </div>
                  <div class="col-4">                  
                     <form class="d-flex" role="search">
                        <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
                        <button class="btn" type="submit">
                           <i class="fa-solid fa-magnifying-glass"></i>
                        </button>
                     </form>
                  </div>
               </div>
            </div>
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
   @import '../../assets/css/variables.scss';

   #navbarSupportedContent {
      div {
         padding: 0 .25rem;
      }

      .icon-box {
         align-content: center;
      }
   }
   
</style>