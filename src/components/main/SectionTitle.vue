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

<style>

</style>