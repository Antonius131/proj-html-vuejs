<template>
   <div class="row">
      <div class="col-12 text-center section-title">
         <h4>{{ subtitle }}</h4>
         <h3>{{ title }}</h3>
      </div>
   </div>
</template>

<script>
export default {
   props: {
      'subtitle': String,
      'title': String
   }
}
</script>

<style lang="scss" scoped>
@import '/src/assets/css/variables.scss';

   .col-12.text-center.section-title {
      padding-left: 4rem;
      padding-right: 4rem;

      h4 {
        color: $brand_secondary;
        font-weight: 300;
        margin-bottom: 1.5rem;
      }

      h3 {
        color: $brand_primary;
      }
   }
</style>