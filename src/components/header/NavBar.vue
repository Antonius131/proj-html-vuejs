<template>
   <nav class="navbar navbar-expand-lg">
      <div class="container-fluid">
         <div class="col-2 logo-box">
            <a class="navbar-brand" href="#">
               <img src="" alt="brand-logo">
            </a>
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
                     <span>
                        <i class="fa-solid fa-circle-user"></i>
                     </span>
                  </div>
                  <div class="col-4 user-search-box">                  
                     <form class="d-flex">
                        <input class="form-control me-2" type="search" placeholder="Search...">
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

      .form-select {
         border: none;

         &:focus {
            box-shadow: none;
         }
      }

      .icon-box {
         text-align: center;

         span {
            width:100%;
            height: 100%;

            i {
               font-size: 1.25rem;
               vertical-align: middle;
               margin-top: .5rem;
            }
         }
      }

      .user-search-box {
         padding: 0 .5rem;
         border-left: 2px solid $border_color;

         .form-control {
            border: none;
            margin-right: 0;
            font-size: $nav_items;

            &:focus {
               box-shadow: none;
            }

            button.btn:hover {
               border-color: transparent;
            }
         }
      }
   }
   
</style>