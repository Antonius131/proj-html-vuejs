<template>
   <div class="row">
      <div class="col-6">
         <div class="card mb-3">
            <div class="row g-0">
               <div class="col-md-4">
                  <h3>22</h3>
                  <p class="card-text"><small>Month</small></p>
                  <SecondaryBtn />
               </div>
               <div class="col-md-8">
                  <div class="card-body">
                     <p class="card-text"><small>City</small></p>
                     <h4 class="card-title">Text</h4>
                  </div>
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

<style>

</style>