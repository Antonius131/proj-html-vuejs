<template>
  <div class="row">
      <div 
         class="col-4"
         v-for="(coach, index) in coachesCards"
         :key="index"
      >
         <div class="card">
            <img :src="coach.imgPath" class="card-img-top" alt="card-image">
            <div class="card-body text-center">
               <h5 class="card-title">
                  {{ coach.title }}
               </h5>
               <p class="card-text">
                  {{ coach.text }}
               </p>
            </div>
            <div class="link-box text-center">
               <a href="#" class="btn go-to-btn">GoTo btn</a>
            </div>
         </div>
      </div>
   </div>
</template>

<script>
export default {
   data: function() {
      return {
         coachesCards: [
            {
               imgPath: require('/src/assets/img/business/home-business-service-slide-01-480x298.jpg'),
               title: 'Consultative Training',
               text: 'With a coach addressing multiple issues that are off balance, affecting your business in various unconsidered ways.'
            },
            {
               imgPath: require('/src/assets/img/business/home-business-service-slide-02-480x298.jpg'),
               title: 'Real Deal Coaching',
               text: 'Brings an exceptionally powerful opportunity. Being able to accept, to work with that opportunity.'
            },
            {
               imgPath: require('/src/assets/img/business/home-business-service-slide-03-480x298.jpg'),
               title: 'Advisor Training Program',
               text: 'Getting high quality, entrepreneur mindset driven online business coaching, is what is needed.'
            },
         ]
      }
   }
}
</script>

<style>

</style>