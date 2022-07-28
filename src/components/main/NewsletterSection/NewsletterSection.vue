<template>
   <section class="newsletter-section">
      <div class="container">
         <div class="row">
            <div class="col-6 offset-3 text-center">
               <h3><strong>Subscribe</strong> Newsletters</h3>
               <p>Enter your email address to register to our new newsletter subscription delivered on a regular basis!</p>
            </div>
         </div>
         <InputText />
      </div>
   </section>
</template>

<script>
import InputText from './InputText.vue';
export default {
    components: { InputText }
}
</script>

<style lang="scss" scoped>
@import '/src/assets/css/variables';

   .newsletter-section {

      h3 {
         color: $brand_secondary;
         font-weight: 400;

         strong {
            color: $text_primary;
         }
      }

      .container {
         background-image: url('/src/assets/img/shapes/maxcoach-shape-09.png');
         background-repeat: no-repeat;
         background-position: right;
         background-size: 18%;
      }
   }
</style>