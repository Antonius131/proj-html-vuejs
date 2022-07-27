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

      <section class="secondary-bg">
         <div class="container">
            <SectionTitle 
               subtitle = "Let's dream big together"
               title= "Explore how can I help you"
            />
            <CoachCards />
         </div>
      </section>

      <section>
         <div class="container">
            <SectionTitle 
               subtitle = "Let's dream big together"
               title= "Explore how can I help you"
            />
            <CourseCards />
         </div>
      </section>
   </main>
</template>

<script>
import BrandCards from './BrandCards.vue'
import SectionTitle from './SectionTitle.vue'
import SecondaryBtn from './SecondaryBtn.vue'
import PrimaryBtn from './PrimaryBtn.vue'
import CoachCards from './CoachCards.vue'
import CourseCards from './CourseCards.vue'

export default {
   components: {
      BrandCards,
      SectionTitle,
      SecondaryBtn,
      PrimaryBtn,
      CoachCards,
      CourseCards
   }
}
</script>

<style lang="scss">
@import '../../assets/css/variables';

   section {
      padding: $section_padding;
   }

   .secondary-bg {
      background-color: $border_color;
   }
</style>