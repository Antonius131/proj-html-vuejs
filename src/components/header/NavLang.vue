<template>
   <select>
      <option>
         <img src="" alt="">
         <p>Flag</p>
      </option>
   </select>
</template>

<script>
export default {
   data: function() {
      return {
         navFlags: [
            {
               value: 'en',
               lang: 'English',
               path: require('../../assets/img/flags/en.png')
            },
            {
               value: 'de',
               lang: 'German',
               path: require('../../assets/img/flags/de.png')
            },
            {
               value: 'fr',
               lang: 'French',
               path: require('../../assets/img/flags/fr.png')
            }
         ]
      }
   }
}
</script>

<style>

</style>