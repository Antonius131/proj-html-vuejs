<template>
   <div class="row">
      <div class="jumbotron">
         <div class="container">
            <div class="row align-items-center">
               <div class="col-6 title-wrap">
                  <h5>
                     New Challenges, New Skills
                  </h5>
                  <h1>
                     Build your own life choaching business
                  </h1>
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

   .row {
      padding: 0;

      .jumbotron {
         background-color: $hero_bg;

         .title-wrap {
            padding-right: 6rem;

            h5 {
               color: $brand_secondary;
               font-weight: 00;
               margin-bottom: 1rem;
            }

            h1 {
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
   }
</style>