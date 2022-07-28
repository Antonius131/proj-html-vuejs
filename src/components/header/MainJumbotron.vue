<template>
   <div class="row">
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
               <div class="col-6 img-wrap">
                  <img class="img-fluid globe-img" src="../../assets/img/hero/home-business-hero-global-image.png" alt="globe-img">
                  <img class="img-fluid avatar-img" src="../../assets/img/hero/home-business-hero-avatar.png" alt="avatar-img">
               </div>            
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

   .row {
      padding: 0;

      .jumbotron {
         background-color: $hero_bg;

         .img-wrap {
            position: relative;
            line-height: 0;

            .globe-img {
               transform: rotate(-45deg);
            }

            .avatar-img {
               position: absolute;
               left: 0;
               bottom: 0;
               height: 100%;
            }
         }
      }
   }
</style>