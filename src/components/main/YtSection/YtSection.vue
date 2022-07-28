<template>
   <section class="yt-section">
      <div class="container">
         <div class="row">
            <div class="col-6">
               <ImgPreview />
            </div>
            <div class="col-6">
               <h2>To thrive in business today, you'll need a good plan</h2>
               <InfoTabs />
            </div>
         </div>
      </div>
   </section>
</template>

<script>
import ImgPreview from './ImgPreview.vue';
import InfoTabs from './InfoTabs.vue';
export default {
    components: { ImgPreview, InfoTabs }
}
</script>

<style lang="scss" scoped>
@import './src/assets/css/variables';

   .yt-section {
      background-color: $yt_bg;
      color: $text_secondary;
      background-image: url(../../../assets/img/video/background-map-dots-top-right-transparent.png);
      background-size: 55%;
      background-repeat: no-repeat;
      background-position-x: right;

      .row {
         background-image: url(../../../assets/img/shapes/maxcoach-shape-07-100x100.png);
         background-size: 10%;
         background-repeat: no-repeat;
         background-position-x: left;
         background-position-y: bottom;
      }

      .col-6 {
         padding: 2rem;
         overflow: auto;

         h2 {
            font-weight: 700;
            margin-bottom: 1rem;
         }
      }
   }

</style>