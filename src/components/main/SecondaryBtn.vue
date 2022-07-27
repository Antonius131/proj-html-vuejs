<template>
   <button type="button" class="btn btn-secondary">
      Secondary Btn
   </button>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
   @import '../../assets/css/variables';

      .btn-secondary {
         color: $brand_secondary;
         font-size: $nav_items;
         background-color: transparent;
         border-color: rgba(33,33,33,.2);
         padding: .75rem 2.5rem;
         margin: 0 .5rem;
         font-weight: 800;


         &:hover {
            background-color: $brand_primary;
            border-color: $brand_primary;
            color: $text_secondary;
         }
      }
</style>