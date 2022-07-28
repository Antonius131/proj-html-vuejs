<template>
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
</template>

<script>
import CourseCards from './CourseCards.vue';
import SectionTitle from '../SectionTitle.vue';
import CaptionText from '../CaptionText.vue';
export default {
    components: { CourseCards, SectionTitle, CaptionText }
}
</script>

<style>

</style>