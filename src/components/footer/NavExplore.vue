<template>
   <div class="row">
      <div class="col-12">
         <h5>Explore</h5>
      </div>
      <div class="col-12">
         <nav class="nav row flex-column">
            <ul>
               <li
                  v-for="(link, index) in exploreItems"
                  :key="index"
               >
                  <a class="nav-link" :href="link.url">{{ link.text }}</a>
               </li>
            </ul>
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

<style lang="scss" scoped>
@import '../../assets/css/variables';

   .nav.row.flex-column {
      padding: 0;

      ul {
         list-style: none;
         margin-bottom: 0;

         a.nav-link {
            padding: .5rem 0;
            color: $text_secondary_rgba;

            &:hover {
               color: $text_secondary;
            }
         }
      }
   }
</style>