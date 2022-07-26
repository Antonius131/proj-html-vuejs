<template>
   <div class="nav-menu">
      <ul>
         <li 
            v-for="item in navMenuItems"
            :key="item"
         >
         <a href="#">{{ item }}</a>
         </li>
      </ul>
   </div>
</template>

<script>
export default {
   data: function() {
      return {
         navMenuItems: {
            _1stItem: 'Home',
            _2ndtItem: 'Pages',
            _3rdItem: 'Courses',
            _4thItem: 'Features',
            _5thItem: 'Blog',
            _6thItem: 'Shop'
         }
      }
   }
}
</script>

<style lang="scss" scoped>
   @import '../../assets/css/mixins.scss';
   @import '../../assets/css/variables.scss';

   .nav-menu {
      text-align: center;

      ul {
         list-style: none;

         li {
            font-size: $nav_items;
            display: inline;
            margin: 0 1rem;

            a {
               color: $brand_primary;
               text-decoration: none;
            }
         }
      }
   }
</style>