<template>
<div class="lang-box">
   <select class="form-select" v-model="selectedLang">
      <option 
         v-for="(lang, index) in navLangs"
         :key="index"
      >
         {{ lang.lang }}
      </option>
   </select>
</div>
</template>

<script>
export default {
   data: function() {
      return {
         selectedLang: 'English',
         navLangs: [
            {
               lang: 'English'
            },
            {
               lang: 'German'
            },
            {
               lang: 'French'
            }
         ]
      }
   }
}
</script>

<style>

</style>