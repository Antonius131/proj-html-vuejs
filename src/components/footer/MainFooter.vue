<template>
   <footer>
      <div class="container">
         <div class="row">
            <div class="col-6">
               <SocialIcons />
            </div>
            <div class="col-6">

            </div>
         </div>
      </div>
   </footer>
</template>

<script>
import SocialIcons from './SocialIcons.vue';

export default {
   components: { 
      SocialIcons
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