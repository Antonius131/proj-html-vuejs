<template>
   <div class="row">
      <div class="col-12">
         <h5>Explore</h5>
      </div>
      <div 
         class="col-12"
         v-for="(link, index) in exploreItems"
         :key="index"
         >
         <nav class="nav row flex-column" >
            <a class="nav-link" :href="link.url">{{ link.text }}</a>
         </nav>
      </div>
   </div>
</template>

<script>
export default {
   data: function() {
      return {
         exploreItems: [
            {
               url: '#',
               text: 'Start Here'
            },
            {
               url: '#',
               text: 'Blog'
            },
            {
               url: '#',
               text: 'About us'
            },
            {
               url: '#',
               text: 'Success story'
            },
            {
               url: '#',
               text: 'Courses'
            },
            {
               url: '#',
               text: 'Contact us'
            },
         ]
      }
   }
}
</script>

<style>

</style>