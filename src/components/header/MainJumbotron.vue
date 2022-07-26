<template>
   <div class="jumbotron">
      <div class="container">
         <SectionTitle />
      </div>
   </div>
</template>

<script>
import SectionTitle from '../main/SectionTitle.vue';

export default {
   components: { 
      SectionTitle 
   }
}
</script>

<style lang="scss" scoped>
   @import '../../assets/css/mixins.scss';
   @import '../../assets/css/variables.scss';

</style>