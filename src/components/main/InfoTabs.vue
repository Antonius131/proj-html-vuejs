<template>
   <div class="accordion">
      <div 
         class="accordion-item"
         v-for="(accordion, index) in infoTabs"
         :key="index"
      >
         <h2 class="accordion-header" id="headingOne">
            <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
               {{ accordion.title }}
            </button>
         </h2>
         <div id="collapseOne" class="accordion-collapse collapse show" aria-labelledby="headingOne" data-bs-parent="#accordionExample">
            <div class="accordion-body">
               {{ accordion.body }}
            </div>
         </div>
      </div>
</div>
</template>

<script>
export default {
   data: function() {
      return {
         infoTabs: [
            {
               title: "How can we help?",
               body: "How many courses you've been on, using however many techniques and methods. Unless you've come to redlize the value of mindset, then you've yet to understand how success comes. With everyone else’s mindset involved impacting too. Hence why business coaching is so crucial for success."
            },
            {
               title: "Why would I need a Business COACH?",
               body: "How many courses you've been on, using however many techniques and methods. Unless you've come to redlize the value of mindset, then you've yet to understand how success comes. With everyone else’s mindset involved impacting too. Hence why business coaching is so crucial for success."
            },
            {
               title: "What is one-on-one coaching?",
               body: "How many courses you've been on, using however many techniques and methods. Unless you've come to redlize the value of mindset, then you've yet to understand how success comes. With everyone else’s mindset involved impacting too. Hence why business coaching is so crucial for success."
            }
         ]
      }
   }
}
</script>

<style>

</style>