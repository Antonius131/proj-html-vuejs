<template>
   <main>
      <BrandSection />
      <CoachesSection />
      <CoursesSection />
      

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
import InfoTabs from './InfoTabs.vue'
import ImgPreview from './ImgPreview.vue'
import EventCards from './EventCards.vue'
import ReviewCards from './ReviewCards.vue'
import InputText from './InputText.vue'
import BrandSection from './BrandSection/BrandSection.vue'
import CoachesSection from './CoachesSection/CoachesSection.vue'
import CoursesSection from './CoursesSection/CoursesSection.vue'

export default {
   components: {
    SectionTitle,
    CaptionText,
    InfoTabs,
    ImgPreview,
    EventCards,
    ReviewCards,
    InputText,
    BrandSection,
    CoachesSection,
    CoursesSection
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
      background-image: url(../../assets/img/video/background-map-dots-top-right-transparent.png);
      background-size: 55%;
      background-repeat: no-repeat;
      background-position-x: right;

      .row {
         background-image: url(../../assets/img/shapes/maxcoach-shape-07-100x100.png);
         background-size: 10%;
         background-repeat: no-repeat;
         background-position-x: left;
         background-position-y: bottom;
      }

      .col-6 {
         padding: 2rem;
         overflow: auto;

         h2 {
            font-weight: 700;
            margin-bottom: 1rem;
         }
      }
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