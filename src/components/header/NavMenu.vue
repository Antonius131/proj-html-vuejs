<template>
   <div class="nav-menu">
      <ul>
         <li 
            v-for="item in navMenuItems"
            :key="item"
         >
         {{ item }}   
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

<style>

</style>