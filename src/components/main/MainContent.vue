<template>
   <main>
      <section>
         <div class="container">
            <div class="row">
               <div class="col-12 text-center section-title">
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

<style lang="scss">
   .col-12.text-center.section-title {
      padding-left: 4rem;
      padding-right: 4rem;
   }
</style>