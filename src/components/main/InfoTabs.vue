<template>
   <div class="accordion accordion-flush">
      <div 
         class="accordion-item"
         v-for="(accordion, index) in infoTabs"
         :key="index"
      >
         <h2 
            class="accordion-header"
            :id="accordion.headId"
         >
            <button 
               class="accordion-button collapsed"
               type="button"
               data-bs-toggle="collapse"
               :data-bs-target="accordion.dataTarget"
               aria-controls="collapseOne"
            >
               {{ accordion.title }}
            </button>
         </h2>
         <div 
            :id="accordion.collapseId"
            class="accordion-collapse collapse"
         >
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
               headId: "flush-headingOne",
               collapseId: "collapseOne",
               dataTarget: "#collapseOne",
               title: "How can we help?",
               body: "How many courses you've been on, using however many techniques and methods. Unless you've come to redlize the value of mindset, then you've yet to understand how success comes. With everyone else’s mindset involved impacting too. Hence why business coaching is so crucial for success."
            },
            {
               headId: "flush-headingTwo",
               collapseId: "collapseTwo",
               dataTarget: "#collapseTwo",
               title: "Why would I need a Business COACH?",
               body: "How many courses you've been on, using however many techniques and methods. Unless you've come to redlize the value of mindset, then you've yet to understand how success comes. With everyone else’s mindset involved impacting too. Hence why business coaching is so crucial for success."
            },
            {
               headId: "flush-headingThree",
               collapseId: "collapseThree",
               dataTarget: "#collapseThree",
               title: "What is one-on-one coaching?",
               body: "How many courses you've been on, using however many techniques and methods. Unless you've come to redlize the value of mindset, then you've yet to understand how success comes. With everyone else’s mindset involved impacting too. Hence why business coaching is so crucial for success."
            }
         ]
      }
   }
}
</script>

<style lang="scss" scoped>
@import '../../assets/css/variables';

</style>