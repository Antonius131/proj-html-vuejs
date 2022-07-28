<template>
   <div class="row">
      <div class="col-12">
         <h5>Address</h5>
         <p>382 NE 191st St # 87394 Miami, FL 33179-3899</p>
         <p>+1(305) 547-9909 (9am - 5pm EST, Monday - Friday)</p>
         <a href="mailto:support@maxcoach.com">support@maxcoach.com</a>
      </div>
   </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import '../../assets/css/variables';

   h5 {
      margin-bottom: 1rem;
   }

   p {
      color: $text_secondary_rgba;
      font-size: $nav_items;
   }

   a {
      text-decoration: none;
      color: $text_secondary_rgba;

      &:hover {
         color: $text_secondary;
      }
   }

</style>