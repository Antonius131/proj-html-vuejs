<template>
   <div class="video-prev py-4">
      <img class="prev-img rounded-2" src="../../assets/img/video/home-business-video-poster-670x450.jpg" alt="yt-prev">
      <img class="ico-img" src="../../assets/img/video/icon-youtube-play.png" alt="yt-ico">
   </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
   .video-prev {
      position: relative;

      img.prev-img {         
         height: 100%;
         width: 100%;
         object-fit: cover;
      }

      img.ico-img {
         position: absolute;
         height: 50px;
         top: calc(50% - 25px);
         left: calc(50% - 38px);
      }
   }
</style>