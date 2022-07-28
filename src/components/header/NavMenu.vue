<template>
   <ul class="navbar-nav me-auto mb-lg-0 d-flex justify-content-center">
      <li 
         class="nav-item"
         v-for="(link, index) in navMenuItems"
         :key="index"
         :class="{ 'dropdown' : link.isDropdown }"
      >
         <a 
            class="nav-link" 
            :href="link.url"
            :class="{ 'dropdown-toggle' : link.isDropdown }"
            :role="link.role"
            :data-bs-toggle="link.toggle"
         >
               {{ link.text }}
         </a>
         <ul class="dropdown-menu">
            <li v-for="(item, index) in link.dropdownMenu" :key="index">
               <a class="dropdown-item" href="#">
                  {{ item.text }}
               </a>
            </li>
         </ul>
      </li>
   </ul>
</template>

<script>
export default {
    data: function () {
        return {
            navMenuItems: [
                {
                  isDropdown: false,
                  role : "",
                  toggle: "",
                  url: "#",
                  text: "Home"
                },
                {
                  isDropdown: false,
                  url: "#",
                  text: "Pages"
                },
                {
                  isDropdown: true,
                  role : "button",
                  toggle: "dropdown",
                  url: "#",
                  text: "Courses",
                  dropdownMenu: [
                     {
                           text: "option"
                     },
                     {
                           text: "option"
                     },
                     {
                           text: "option"
                     }
                  ]
                },
                {
                  isDropdown: false,
                  role : "",
                  toggle: "",
                  url: "#",
                  text: "Features"
                },
                {
                  isDropdown: false,
                  role : "",
                  toggle: "",
                  url: "#",
                  text: "Blog"
                },
                {
                  isDropdown: false,
                  role : "",
                  toggle: "",
                  url: "#",
                  text: "Shop"
                }
            ]
        };
    }
}
</script>

<style lang="scss" scoped>
   @import '../../assets/css/variables.scss';

   ul {
      list-style: none;

      li.nav-item {
         display: inline;
         margin: 0 .5rem;

         .nav-link {
            color: $text_primary;
            text-decoration: none;
         }
      }
   }
</style>