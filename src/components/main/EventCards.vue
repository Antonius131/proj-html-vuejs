<template>
   <div class="row">
      <div 
         class="col-6"
         v-for="(event, index) in eventCards"
         :key="index"
      >
         <div class="card mb-3">
            <div class="row g-0">
               <div class="col-md-9">
                  <div class="card-body">
                     <p class="card-text"><small>{{ event.place }}</small></p>
                     <h5 class="card-title">{{ event.title }}</h5>
                  </div>
               </div>
               <div class="col-md-3 text-center">
                  <h3 class="card-title">{{ event.day }}</h3>
                  <p class="card-text"><small>{{ event.month }}</small></p>
                  <PrimaryBtn 
                     text = "Get Ticket"   
                  />
               </div>
            </div>
         </div>
      </div>
   </div>
</template>

<script>
import PrimaryBtn from './PrimaryBtn.vue';

export default {
   components: { 
      PrimaryBtn 
   },
   data: function() {
      return {
         eventCards: [
            {
               place: 'Texas, US',
               title: 'Storytelling Workshop',
               day: '22',
               month: 'NOV'
            },
            {
               place: 'New York, US',
               title: 'Painting Art Contest 2020',
               day: '10',
               month: 'OCT'
            },
            {
               place: 'Hamburg, Germany',
               title: 'International Art Fair 2020',
               day: '23',
               month: 'NOV'
            },
            {
               place: 'Illinois, US',
               title: 'Street Performance, Call For Artist',
               day: '15',
               month: 'DEC'
            },
            {
               place: 'Illinois, US',
               title: 'Consumer Food Safety Education Conference',
               day: '22',
               month: 'JUL'
            },
            {
               place: 'Dubai',
               title: 'How Meditation Improve Your Mental Healt',
               day: '12',
               month: 'AUG'
            }
         ]
      }
   }
}
</script>

<style lang="scss" scoped>
@import '../../assets/css/variables';

   .card {
      background-color: $border_color;
      border: none;
   }

</style>