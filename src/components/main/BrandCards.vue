<template>
   <div class="row">
      <div class="col-4">
         <div class="card mb-3">
            <div class="row g-0">
               <div class="col-md-4">
                  <i>icon</i>
               </div>
               <div class="col-md-8">
                  <div class="card-body">
                     <h5 class="card-title">Title</h5>
                     <p class="card-text">Subtitle</p>
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
         brandCards: [
            {
               title: 'One to One',
               subtitle: 'Getting the necessary clarity about the current state to help you improve your game.'
            },
            {
               title: 'Anywhere',
               subtitle: 'Access to valuable and portable program which allow you to setup and live anywhere you want.'
            },
            {
               title: 'On time',
               subtitle: 'Punctuality is our top priority because it\'s an essential criteria to assess a program quality.'
            },
            {
               title: 'Online Courses',
               subtitle: 'Online business coaching now offers you a very powerful way to empower your business into success.'
            },
            {
               title: 'Consulting',
               subtitle: 'You will get a clear sense of direction for your business, thorough assessment and faster results.'
            },
            {
               title: 'Self Development',
               subtitle: 'Business Coaching often keep your focus and develop you both in a professional and personal way.'
            },
         ]
      }
   }
}
</script>

<style>

</style>