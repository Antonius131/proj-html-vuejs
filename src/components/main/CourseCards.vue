<template>
   <div class="row">
      <div 
         class="col-3"
         v-for="(course, index) in coursesCards"
         :key="index"
      >
         <div class="card">
            <img :src="course.imgPath" class="card-img" alt="card-img">
            <div class="card-img-overlay">
               <div class="card-body text-white">
                  <h6 class="card-title">{{ course.price }}</h6>
                  <p class="card-text">{{ course.text }}</p>
                  <div class="course-caption">
                     <span>
                        {{ course.lessons }}
                     </span>
                     <span>
                        {{ course.students }}
                     </span>
                     <p>
                        {{ course.purpose }}
                     </p>
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
         coursesCards: [
            {
               imgPath: require('/src/assets/img/courses/course-02-443x600.jpg'),
               price: '$40.00',
               text: 'Learning to Write as a Professional Author',
               lessons: '20 Lessons',
               students: '50 Students',
               purpose: 'The purpose of this course is to provide the for inspiring readers and...'
            },
            {
               imgPath: require('/src/assets/img/courses/stock-full-hd-03-443x600.jpg'),
               price: 'Free',
               text: 'Customer-centric Info-Tech Strategies',
               lessons: '20 Lessons',
               students: '50 Students',
               purpose: 'The purpose of this course is to provide the for inspiring readers and...'
            },
            {
               imgPath: require('/src/assets/img/courses/stock-full-hd-04-443x600.jpg'),
               price: '$19.00',
               text: 'Open Programming Courses for Everyone: Python',
               lessons: '20 Lessons',
               students: '50 Students',
               purpose: 'The purpose of this course is to provide the for inspiring readers and...'
            },
            {
               imgPath: require('/src/assets/img/courses/stock-full-hd-06-443x600.jpg'),
               price: '$26.00',
               text: 'Academic Listening and Note-taking',
               lessons: '20 Lessons',
               students: '50 Students',
               purpose: 'The purpose of this course is to provide the for inspiring readers and...'
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

      .card {
         border: none;

         .card-img-overlay {
            background: linear-gradient(0deg, rgba(0,0,0,.95) 0%, rgba(33,33,33,0.4) 40%, rgba(255,255,255,0) 100%);

            .card-body {
               position: absolute;
               bottom: 0;
               left: 0;

               h6,
               p {
                  font-weight: 800;
               }

               h6 {
                  color: $brand_secondary;
               }
               
            }
         }
      }
   }


</style>