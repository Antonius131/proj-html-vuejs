<template>
   <main>
      <section>
         <div class="container">
            <div class="row">
               <div class="col-12 text-center">
                  <h4>Let's dream big together</h4>
                  <h3>We are pioneers of the digital approach, using leading-edge technology to simplify procedures and apply executive coaching in the new age of digitalization.</h3>
               </div>
            </div>
            <BrandCards />
         </div>
      </section>
   </main>
</template>

<script>
import BrandCards from './BrandCards.vue'

export default {
   components: {
      BrandCards
   },
   data: function() {
      return {
         sectionTitles: [
            {
               id: 1,
               subtitle: 'Let\'s dream big together',
               title: ''
            },
            {
               id: 2,
               subtitle: 'Let\'s dream big together',
               title: 'Explore how can I help you'
            },

         ]
      }
   }
}
</script>

<style>

</style>