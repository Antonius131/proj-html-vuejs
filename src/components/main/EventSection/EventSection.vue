<template>
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
</template>

<script>
import SectionTitle from '../SectionTitle.vue';
import EventCards from './EventCards.vue';
import CaptionText from '../CaptionText.vue';
export default {
    components: { SectionTitle, EventCards, CaptionText }
}
</script>

<style>

</style>