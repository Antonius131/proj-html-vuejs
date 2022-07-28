<template>
   <main>
      <BrandSection />
      <CoachesSection />
      <CoursesSection />
      <YtSection />

      <section>
         <div class="container">
            <SectionTitle
               subtitle = "Wanna transform your life?"
               title= "Upcoming Events"
            />
            <EventCards />
            <CaptionText 
               text = "Excited about our event?"
               link = "View all events"
            />
         </div>
      </section>

      <section class="secondary-bg">
         <div class="container-fluid">
            <SectionTitle
               subtitle = "People are praising Maxcoach"
               title= "What make they love us?"
            />
            <ReviewCards />
         </div>
      </section>

      <section class="newsletter-section">
         <div class="container">
            <div class="row">
               <div class="col-6 offset-3 text-center">
                  <h3><strong>Subscribe</strong> Newsletters</h3>
                  <p>Enter your email address to register to our new newsletter subscription delivered on a regular basis!</p>
               </div>
            </div>
            <InputText />
         </div>
      </section>
   </main>
</template>

<script>
import SectionTitle from './SectionTitle.vue'
import CaptionText from './CaptionText.vue'
import EventCards from './EventCards.vue'
import ReviewCards from './ReviewCards.vue'
import InputText from './InputText.vue'
import BrandSection from './BrandSection/BrandSection.vue'
import CoachesSection from './CoachesSection/CoachesSection.vue'
import CoursesSection from './CoursesSection/CoursesSection.vue'
import YtSection from './YtSection/YtSection.vue'

export default {
   components: {
    SectionTitle,
    CaptionText,
    EventCards,
    ReviewCards,
    InputText,
    BrandSection,
    CoachesSection,
    CoursesSection,
    YtSection
}
}
</script>

<style lang="scss" scoped>
@import './src/assets/css/variables';

   section {
      padding: $section_padding;
   }

   .secondary-bg {
      background-color: $border_color;
   }

   .newsletter-section {

      h3 {
         color: $brand_secondary;
         font-weight: 400;

         strong {
            color: $text_primary;
         }
      }

      .container {
         background-image: url('/src/assets/img/shapes/maxcoach-shape-09.png');
         background-repeat: no-repeat;
         background-position: right;
         background-size: 18%;
      }
   }
</style>