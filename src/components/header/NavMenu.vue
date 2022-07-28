<template>
   <ul class="navbar-nav me-auto mb-lg-0 d-flex justify-content-center">
      <li 
         class="nav-item"
         v-for="(link, index) in navMenuItems"
         :key="index"
      >
         <a class="nav-link" :href="link.url">{{ link.text }}</a>
      </li>
   </ul>
</template>

<script>
export default {
   data: function() {
      return {
         navMenuItems: [
            {
               url: '#',
               text: 'Home'
            },
            {
               url: '#',
               text: 'Pages'
            },
            {
               url: '#',
               text: 'Courses'
            },
            {
               url: '#',
               text: 'Features'
            },
            {
               url: '#',
               text: 'Blog'
            },
            {
               url: '#',
               text: 'Shop'
            }
         ]
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