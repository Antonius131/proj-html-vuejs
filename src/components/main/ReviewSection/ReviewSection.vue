<template>
   <section class="secondary-bg">
      <div class="container-fluid">
         <SectionTitle 
            subtitle = "People are praising Maxcoach"
            title= "What make they love us?"
         />
         <ReviewCards />
      </div>
   </section>
</template>

<script>
import ReviewCards from './ReviewCards.vue';
import SectionTitle from '../SectionTitle.vue';
export default {
    components: { ReviewCards, SectionTitle }
}
</script>

<style>

</style>