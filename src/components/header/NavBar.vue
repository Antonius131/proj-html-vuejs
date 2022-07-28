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
               <div class="col-4 d-flex">
                  <div class="col-6">                  
                     <select class="form-select">
                        <option selected>English</option>
                        <option value="1">German</option>
                        <option value="2">French</option>
                     </select>
                  </div>
                  <div class="col-6">                  
                     <form class="d-flex" role="search">
                        <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
                        <button class="btn btn-outline-success" type="submit">Search</button>
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

   
</style>