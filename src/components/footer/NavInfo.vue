<template>
   <div class="row">
      <div class="col-12">
         <h5>Informations</h5>
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
               text: 'Membership'
            },
            {
               url: '#',
               text: 'Purchase guides'
            },
            {
               url: '#',
               text: 'Privacy policy'
            },
            {
               url: '#',
               text: 'Terms of service'
            }
         ]
      }
   }
}
</script>

<style lang="scss" scoped>
@import '../../assets/css/variables';

   ul {
      list-style: none;

      a.nav-link {
         padding: .5rem 0;
         color: $text_secondary_rgba;

         &:hover {
            color: $text_secondary;
         }
      }
   }

</style>