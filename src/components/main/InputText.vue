<template>
   <div class="row">
      <div class="col-6 offset-3">
         <div class="input-group mb-3">
            <input 
               type="text"
               class="form-control" 
               placeholder="Enter your email" 
            >
            <button type="button" class="btn btn-primary">Subscribe</button>
         </div>
      </div>
   </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import '/src/assets/css/variables.scss';

   .row {
      padding-top: 0;
      background-image: url('/src/assets/img/shapes/maxcoach-shape-02.png');
      background-repeat: no-repeat;
      background-size: 8%;
      background-position-x: right;
      background-position-y: top;

      input.form-control {
         padding: .75rem 1rem;
         background-color: $border_color;
      }

      .btn-primary {
         background-color: $brand_secondary;
         border: none;
         padding: 0 1.25rem;
      }
   }
   

</style>