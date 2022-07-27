<template>
   <div class="row">
      <div class="col-4 offset-4 text-center">
         <p>{{ text }} <a href="#">{{ link }}</a></p>
      </div>
   </div>
</template>

<script>
export default {
   props: {
      'text': String,
      'link': String
   }
}
</script>

<style lang="scss" scoped>
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