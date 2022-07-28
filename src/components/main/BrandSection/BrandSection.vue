<template>
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
</template>

<script>
import BrandCards from './BrandCards.vue';
import SectionTitle from '../SectionTitle.vue';
import PrimaryBtn from '../PrimaryBtn.vue';
import SecondaryBtn from '../SecondaryBtn.vue';

export default {
    components: { BrandCards, SectionTitle, PrimaryBtn, SecondaryBtn }
}
</script>

<style>

</style>