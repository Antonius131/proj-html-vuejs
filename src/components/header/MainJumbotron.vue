<template>
   <div class="jumbotron">
      <div class="container">
         <div class="row">
            <div class="col-6 wrap title-wrap">
               <SectionTitle 
                  subtitle = "New Challenges, New Skills"
                  title = "Build your own life choaching business"
                  paragraph = "Whole-Life Business Coaching for committed entrepreneurs"
               />
            </div>
            <div class="col-6 wrap img-wrap">
               <!-- <img src="../../assets/img/hero/home-business-hero-avatar.png" alt="avatar"> -->
            </div>            
         </div>
      </div>
   </div>
</template>

<script>
import SectionTitle from '../main/SectionTitle.vue';

export default {
    components: { SectionTitle }
}
</script>

<style lang="scss" scoped>
   @import '../../assets/css/variables.scss';

   .jumbotron {
      background-color: $hero_bg;
   }
</style>