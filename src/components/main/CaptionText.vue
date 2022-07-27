<template>
   <div class="row">
      <div class="col-12 text-center">
         <p>Caption text <a href="#">Link</a></p>
      </div>
   </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoper>
@import '../../assets/css/variables';

   p {
      color: $text_primary_rgba;

      a {
         color: $text_primary;
         text-decoration-color: $text_primary_rgba;

         &:hover {
            color: $brand_secondary;
            text-decoration-color: $brand_secondary;
         }
      }
   }


</style>