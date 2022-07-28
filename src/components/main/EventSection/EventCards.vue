<template>
   <div class="row">
      <div 
         class="col-6"
         v-for="(event, index) in eventCards"
         :key="index"
      >
         <div class="card mb-4">
            <div class="row g-0">
               <div class="col-md-8 event-title-box">
                  <p class="card-text"><small>{{ event.place }}</small></p>
                  <h5 class="card-title">{{ event.title }}</h5>
               </div>
               <div class="col-md-4 text-center event-date-box">
                  <h1 class="card-title">{{ event.day }}</h1>
                  <p class="card-text"><small>{{ event.month }}</small></p>
                  <button type="button" class="btn btn-primary">Get Tickets</button>
               </div>
            </div>
         </div>
      </div>
   </div>
</template>

<script>
export default {
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
@import '/src/assets/css/variables';

   .card {
      background-color: $border_color;
      border: none;
      padding: 0 2rem;

      &:hover {
         cursor: pointer;
         background-color: #fff;
         border-left: 2px solid $brand_secondary;
         box-shadow: $box_shadow;

         button.btn {
            background-color: $brand_primary;
         }
      }

      .event-title-box {
         padding: 0;

         .card-text {
            color: $text_primary_rgba;
            margin-bottom: .25rem;
         }

         .card-title {
            font-weight: 800;
         }
      }

      .event-date-box {
         padding: 0;

         .card-title {
            color: $brand_secondary;
            font-size: 3rem;
            margin-bottom: 0;
         }

         p.card-text {
            font-weight: 900;
            margin-bottom: .5rem;
         }

         button {
            padding: .25rem 1.75rem;
            background-color: $brand_secondary;
            border: none;
         }
      }
   }

</style>