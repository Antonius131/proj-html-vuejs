<template>
   <div class="accordion">
      <div class="accordion-item">
         <h2 class="accordion-header" id="headingOne">
            <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
               Accordion Item 
            </button>
         </h2>
         <div id="collapseOne" class="accordion-collapse collapse show" aria-labelledby="headingOne" data-bs-parent="#accordionExample">
            <div class="accordion-body">
               text
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
               titleItem: "How can we help?",
               body: "How many courses you've been on, using however many techniques and methods. Unless you've come to redlize the value of mindset, then you've yet to understand how success comes. With everyone else’s mindset involved impacting too. Hence why business coaching is so crucial for success."
            },
            {
               titleItem: "Why would I need a Business COACH?",
               body: "How many courses you've been on, using however many techniques and methods. Unless you've come to redlize the value of mindset, then you've yet to understand how success comes. With everyone else’s mindset involved impacting too. Hence why business coaching is so crucial for success."
            },
            {
               titleItem: "What is one-on-one coaching?",
               body: "How many courses you've been on, using however many techniques and methods. Unless you've come to redlize the value of mindset, then you've yet to understand how success comes. With everyone else’s mindset involved impacting too. Hence why business coaching is so crucial for success."
            }
         ]
      }
   }
}
</script>

<style>

</style>