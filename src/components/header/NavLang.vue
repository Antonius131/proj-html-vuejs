<template>
   <select class="form-select">
      <option 
         v-for="(lang, index) in navLangs"
         :key="index"
         :value="lang.value"
      >
         <p>
            {{ lang.lang }}
         </p>
      </option>
   </select>
</template>

<script>
export default {
   data: function() {
      return {
         navLangs: [
            {
               value: 'en',
               lang: 'English'
            },
            {
               value: 'de',
               lang: 'German'
            },
            {
               value: 'fr',
               lang: 'French'
            }
         ]
      }
   },
   methods: {
      getFlag() {
         console.log(this.navLangs);
         for (let i = 0; i < this.navLangs.length; i++) {
            const value = this.navLangs[i].value;
            console.log(value);
            return value;
         }
      }
   }
}
</script>

<style>

</style>