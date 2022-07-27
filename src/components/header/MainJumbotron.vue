<template>
   <div class="jumbotron">
      <div class="container">
         <div class="row">
            <div class="col-6 wrap title-wrap">
               <SectionTitle />
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
   components: { 
      SectionTitle 
   }
}
</script>

<style lang="scss" scoped>
   @import '../../assets/css/mixins';
   @import '../../assets/css/variables.scss';

   .jumbotron {
      background-color: $hero_bg;

      .wrap {
         width: 50%;
         height: 100%;
      }

      .img-wrap {
         background-image: url(../../assets/img/hero/home-business-hero-global-image.png);
         background-size: contain;
         background-repeat: no-repeat;
         padding-top: 3rem;
         line-height: 0;
         height: 100%;
      }
   }
</style>