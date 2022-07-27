<template>
   <main>
      <section>
         <div class="container">
            <SectionTitle 
               subtitle = "Let's dream big together"
               title= "We are pioneers of the digital approach, using leading-edge technology to simplify procedures and apply executive coaching in the new age of digitalization."
            />
            <BrandCards />
         </div>
      </section>
   </main>
</template>

<script>
import BrandCards from './BrandCards.vue'
import SectionTitle from './SectionTitle.vue'

export default {
   components: {
      BrandCards,
      SectionTitle
   }
}
</script>

<style lang="scss">
</style>