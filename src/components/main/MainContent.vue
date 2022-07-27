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
         <div class="container-fluid">
            <SectionTitle 
               subtitle = "Let's dream big together"
               title= "Explore how can I help you"
            />
            <CourseCards />
            <CaptionText 
               text = "Take the control of their life back and start doing things to make their dream come true."
               link = "View all courses"
            />
         </div>
      </section>

      <section class="yt-section">
         <div class="container">
            <div class="row">
               <div class="col-6">
                  <ImgPreview />
               </div>
               <div class="col-6">
                  <h2>To thrive in business today, you'll need a good plan</h2>
                  <InfoTabs />
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
import CoachCards from './CoachCards.vue'
import CourseCards from './CourseCards.vue'
import CaptionText from './CaptionText.vue'
import InfoTabs from './InfoTabs.vue'
import ImgPreview from './ImgPreview.vue'

export default {
   components: {
      BrandCards,
      SectionTitle,
      SecondaryBtn,
      PrimaryBtn,
      CoachCards,
      CourseCards,
      CaptionText,
      InfoTabs,
      ImgPreview
   }
}
</script>

<style lang="scss" scoped>
@import '../../assets/css/variables';

   section {
      padding: $section_padding;
   }

   .secondary-bg {
      background-color: $border_color;
   }

   .yt-section {
      background-color: $yt_bg;
      color: $text_secondary;

      .col-6 {
         padding: 2rem;
         overflow: auto;

         h2 {
            font-weight: 700;
            margin-bottom: 1rem;
         }
      }

   }
</style>