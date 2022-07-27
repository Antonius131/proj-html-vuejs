<template>
   <div class="row">
      <div class="col-6">
         <div class="card mb-3">
            <div class="row g-0">
               <div class="col-md-9">
                  <div class="card-body">
                     <p class="card-text"><small>City</small></p>
                     <h4 class="card-title">Text</h4>
                  </div>
               </div>
               <div class="col-md-3 text-center">
                  <h3 class="card-title">22</h3>
                  <p class="card-text"><small>Month</small></p>
                  <SecondaryBtn />
               </div>
            </div>
         </div>
      </div>
   </div>
</template>

<script>
import SecondaryBtn from './SecondaryBtn.vue';

export default {
   components: { 
      SecondaryBtn 
   }
}
</script>

<style lang="scss" scoped>
@import '../../assets/css/variables';

   .card {
      background-color: $bg_secondary;
      border: none;
   }

</style>