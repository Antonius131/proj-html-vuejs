<template>
   <div class="row">
      <div class="col-4">
         <div 
            class="card"
            v-for="(review, index) in reviewCards"
            :key="index"
         >
            <div class="card-body">
               <h5 class="card-title">{{ rieview.title }}</h5>
               <p class="card-text">{{ review.text }}</p>
               <div class="user-review-box">
                  <img 
                     class="rounded-circle" 
                     :src="review.imgPath" 
                     alt="review-img">
                  <h6 class="card-title">{{ review.name }}</h6>
                  <p><small>{{ review.job }}</small></p>
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

<style>

</style>