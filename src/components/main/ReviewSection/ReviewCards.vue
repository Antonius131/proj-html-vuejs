<template>
   <div class="row">
      <div 
         class="col-4"
         v-for="(review, index) in reviewCards"
         :key="index"
         :class="{ inactive : !review.isActive }"
      >
         <div class="card">
            <div class="card-body">
               <h5 class="card-title">{{ review.title }}</h5>
               <p class="card-text">{{ review.text }}</p>
               <div class="row user-review-box mt-4">
                  <div class="col-3">
                     <img 
                        class="rounded-circle img-fluid" 
                        :src="review.imgPath" 
                        alt="review-img"
                     >
                  </div>
                  <div class="col-9">
                     <h6>{{ review.name }}</h6>
                     <p><small>{{ review.job }}</small></p>
                  </div>
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
         reviewCards: [
            {
               title: 'It\'s a choice of quality for people with special needs.',
               text: 'I\'m a very strict person so I require everything to be organized and neat. Then, I\'ll be able to make things right and shine. MaxCoach guys just got me.',
               name: 'Florence Themes',
               job: '/ Multimedia Admin',
               imgPath: require('/src/assets/img/reviews/testimonial-avata-03.jpg'),
               isActive: false
            },
            {
               title: 'It\'s a choice of quality for people with special needs.',
               text: 'I\'m a very strict person so I require everything to be organized and neat. Then, I\'ll be able to make things right and shine. MaxCoach guys just got me.',
               name: 'Florence Themes',
               job: '/ Multimedia Admin',
               imgPath: require('/src/assets/img/reviews/testimonial-avata-02.jpg'),
               isActive: true
            },
            {
               title: 'It\'s a choice of quality for people with special needs.',
               text: 'I\'m a very strict person so I require everything to be organized and neat. Then, I\'ll be able to make things right and shine. MaxCoach guys just got me.',
               name: 'Florence Themes',
               job: '/ Multimedia Admin',
               imgPath: require('/src/assets/img/reviews/testimonial-avata-01.jpg'),
               isActive: false
            },
         ]
      }
   }
}
</script>

<style lang="scss" scoped>
@import '/src/assets/css/variables';
   
   .row {
      padding: 2rem 4rem;

      .card {
         padding: 2rem;

         &:hover {
            cursor: pointer;
         }

         .card-title {
            font-weight: 700;
         }

         .card-text {
            color: $text_primary_rgba;
         }
      }

      .user-review-box {
         padding: 0;

         h6 {
            text-transform: uppercase;
            font-weight: 700;
            font-size: $nav_items;
         }

         p {
            color: $text_primary_rgba;
         }
      }

      .inactive {
         opacity: .2;
      }
   }

</style>