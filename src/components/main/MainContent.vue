<template>
   <main>
      <BrandSection />
      <CoachesSection />
      <CoursesSection />
      <YtSection />
      <EventSection />
      <ReviewSection />
      <NewsletterSection /> 
   </main>
</template>

<script>
import BrandSection from './BrandSection/BrandSection.vue'
import CoachesSection from './CoachesSection/CoachesSection.vue'
import CoursesSection from './CoursesSection/CoursesSection.vue'
import YtSection from './YtSection/YtSection.vue'
import EventSection from './EventSection/EventSection.vue'
import ReviewSection from './ReviewSection/ReviewSection.vue'
import NewsletterSection from './NewsletterSection/NewsletterSection.vue'

export default {
   components: {
      BrandSection,
      CoachesSection,
      CoursesSection,
      YtSection,
      EventSection,
      ReviewSection,
      NewsletterSection
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
</style>