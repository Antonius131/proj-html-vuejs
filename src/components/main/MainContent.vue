<template>
   <main>
      <section>
         <div class="container">
            <SectionTitle 
               subtitle = "Let's dream big together"
               title= "We are pioneers of the digital approach, using leading-edge technology to simplify procedures and apply executive coaching in the new age of digitalization."
            />
            <BrandCards />
            <div class="row">
               <div class="col-12 text-center">
                  <SecondaryBtn 
                     text = "Learn more"   
                  />
                  <PrimaryBtn 
                     text = "Get started today"
                  />
               </div>
            </div>
         </div>
      </section>
   </main>
</template>

<script>
import BrandCards from './BrandCards.vue'
import SectionTitle from './SectionTitle.vue'
import SecondaryBtn from './SecondaryBtn.vue'
import PrimaryBtn from './PrimaryBtn.vue'

export default {
   components: {
    BrandCards,
    SectionTitle,
    SecondaryBtn,
    PrimaryBtn
}
}
</script>

<style lang="scss">
</style>