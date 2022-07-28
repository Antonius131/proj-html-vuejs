<template>
   <footer>
      <div class="container">
         <div class="row">
            <div class="col-8">
               <BrandAddress />
               <SocialIcons />
            </div>
            <div class="col-2">
               <NavExplore />
            </div>
            <div class="col-2">
               <NavInfo />
            </div>
         </div>
         <div class="row brand-caption">
            <div class="col-12 text-center">
               <p>© 2020 Maxcoach. All Rights Reserved</p>
            </div>
         </div>
      </div>
   </footer>
</template>

<script>
import SocialIcons from './SocialIcons.vue';
import BrandAddress from './BrandAddress.vue';
import NavExplore from './NavExplore.vue';
import NavInfo from './NavInfo.vue';

export default {
   components: {
    SocialIcons,
    BrandAddress,
    NavExplore,
    NavInfo,
}
}
</script>

<style lang="scss">
@import '../../assets/css/variables';

   footer {
      background-color: $brand_primary;
      color: $text-secondary;
      padding: $section_padding;

      .row {
         padding: 0;
      }

      .brand-caption {
         color: $text_secondary_rgba;
      }
   }
</style>