<template>
   <div class="row">
      <div 
         class="col-3"
         v-for="(course, index) in coursesCards"
         :key="index"
      >
         <div class="card rounded-0">
            <img :src="course.imgPath" class="card-img" alt="card-img">
            <div class="card-img-overlay">
               <h5 class="card-title">{{ course.price }}</h5>
               <p class="card-text">{{ course.text }}</p>
            </div>
         </div>
      </div>
   </div>
</template>

<script>
export default {
   data: function() {
      return {
         coursesCards: [
            {
               imgPath: require('/src/assets/img/courses/course-02-443x600.jpg'),
               price: '$40.00',
               text: 'Learning to Write as a Professional Author'
            },
            {
               imgPath: require('/src/assets/img/courses/stock-full-hd-03-443x600.jpg'),
               price: 'Free',
               text: 'Customer-centric Info-Tech Strategies'
            },
            {
               imgPath: require('/src/assets/img/courses/stock-full-hd-04-443x600.jpg'),
               price: '$19.00',
               text: 'Open Programming Courses for Everyone: Python'
            },
            {
               imgPath: require('/src/assets/img/courses/stock-full-hd-06-443x600.jpg'),
               price: '$26.00',
               text: 'Academic Listening and Note-taking'
            }
         ]
      }
   }
}
</script>

<style lang="scss" scoped>
@import '../../assets/css/variables';

   .row {
      padding: 2rem 4rem;
   }

   .card {
      height: 400px;
   }

</style>