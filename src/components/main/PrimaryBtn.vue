<template>
   <button type="button" class="btn btn-primary">
      {{ text }}
   </button>
</template>

<script>
export default {
   props: {
      'text': String
   }
}
</script>

<style lang="scss" scoped>
   @import '../../assets/css/variables';

      .btn-primary {
         background-color: $brand_secondary;
         border-color: $brand_secondary;
         font-size: $nav_items;
         padding: .75rem 2.5rem;
         margin: 0 .5rem;
         font-weight: 800;

         &:hover {
            background-color: $brand_primary;
            border-color: $brand_primary;
         }
      }
</style>