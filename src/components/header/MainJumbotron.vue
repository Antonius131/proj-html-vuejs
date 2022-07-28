<template>
   <div class="jumbotron">
      <div class="container">
         <div class="row align-items-center">
            <div class="col-6 title-wrap">
               <h5>
                  New Challenges, New Skills
               </h5>
               <h2>
                  Build your own life choaching business
               </h2>
               <p>
                  Whole-Life Business Coaching for committed entrepreneurs
               </p>
               <PrimaryBtn 
                  text = "Get started today"
               />
            </div>
            <div class="col-6 img-wrap">
               <img class="img-fluid globe-img" src="../../assets/img/hero/home-business-hero-global-image.png" alt="globe-img">
               <img class="img-fluid avatar-img" src="../../assets/img/hero/home-business-hero-avatar.png" alt="avatar-img">
            </div>            
         </div>
      </div>
   </div>
</template>

<script>
import PrimaryBtn from '../main/PrimaryBtn.vue';

export default {
   components: { 
      PrimaryBtn 
   }
}
</script>

<style lang="scss" scoped>
   @import '../../assets/css/variables.scss';

   .jumbotron {
      background-color: $hero_bg;

      .row {
         padding-top: 2rem;
         padding-bottom: 0;
      }

      .title-wrap {
         padding-right: 6rem;

         h5 {
            color: $brand_secondary;
            font-weight: 00;
            margin-bottom: 1rem;
         }

         h2 {
            color: $brand_primary;
            text-transform: uppercase;
            font-weight: 800;
         }

         p {
            color: $text_primary_rgba;
         }
      }

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
</style>