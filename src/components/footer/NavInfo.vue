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

<style>

</style>