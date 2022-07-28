<template>
   <section class="secondary-bg">
      <div class="container">
         <SectionTitle
            subtitle = "Let's dream big together"
            title= "Explore how can I help you"
         />
         <CoachCards />
      </div>
   </section>
</template>

<script>
import SectionTitle from '../SectionTitle.vue';
import CoachCards from '../CoachCards.vue';
export default {
    components: { SectionTitle, CoachCards }
}
</script>

<style>

</style>