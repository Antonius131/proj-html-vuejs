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
    NavInfo
}
}
</script>

<style lang="scss">
@import '../../assets/css/variables';

   footer {
      background-color: $brand_primary;
      color: $text-secondary;
      padding: $section_padding;
   }

</style>