<template>
   <div class="row">
      <div class="col-10 offset-1 text-center section-title">
         <h5>{{ subtitle }}</h5>
         <h3>{{ title }}</h3>
         <p> {{ paragraph }}</p>
      </div>
   </div>
</template>

<script>
export default {
   props: {
      'subtitle': String,
      'title': String,
      'paragraph': String
   }
}
</script>

<style lang="scss" scoped>
@import '/src/assets/css/variables.scss';

   h5 {
      color: $brand_secondary;
      font-weight: 300;
      margin-bottom: 1rem;
   }

   h3 {
      color: $brand_primary;
   }

   p {
      color: $text_primary_rgba;
   }
</style>