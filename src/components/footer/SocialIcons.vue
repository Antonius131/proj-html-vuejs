<template>
   <div class="row">
      <div class="col-12">
         <div 
            class="icon-box"
            v-for="brand in socialIcons"
            :key="brand"
         >
            <i 
               class="fa-brands"
               :class="brand"
            >
            </i>
         </div>
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

<style>

</style>