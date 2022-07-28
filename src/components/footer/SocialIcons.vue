<template>
   <div class="row">
      <div class="col-12">
         <span 
            class="icon-box"
            v-for="brand in socialIcons"
            :key="brand"
         >
            <i 
               class="fa-brands"
               :class="brand"
            >
            </i>
         </span>
      </div>
   </div>
</template>

<script>
export default {
   data: function() {
      return {
         socialIcons: [
            'fa-facebook',
            'fa-twitter',
            'fa-instagram',
            'fa-linkedin'
         ]
      }
   }
}
</script>

<style lang="scss" scoped>
@import '../../assets/css/variables';

   .icon-box {
      padding: 1rem .5rem;
      color: $text_secondary_rgba;
   }

</style>