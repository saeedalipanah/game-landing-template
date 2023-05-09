<template>
  <div class="game-gallery-bg">
  <div class="container game-gallery-area">
    <div class="slider-wrapper">
      <img src="img/images/game_gallery_01.png" alt="" />
      <img src="img/images/game_gallery_02.png" alt="" />
      <img src="img/images/game_gallery_03.png" alt="" />
      <img src="img/images/game_gallery_04.png" alt="" />
    </div>
      <i class="action-btn prev fa-sharp fa-solid fa-circle-chevron-left" @click="prev"></i>
      <i class="action-btn next fa-sharp fa-solid fa-circle-chevron-right" @click="next"></i>
  </div>
  
  </div>
</template>

<script>
export default {
  methods: {
    next() {
      const sliderWrapper = document.querySelector(".slider-wrapper");
      sliderWrapper.scrollTo({
        left: sliderWrapper.scrollLeft + sliderWrapper.clientWidth,
        behavior: "smooth",
      });
    },
    prev() {
      const sliderWrapper = document.querySelector(".slider-wrapper");
      sliderWrapper.scrollTo({
        left: sliderWrapper.scrollLeft - sliderWrapper.clientWidth,
        behavior: "smooth",
      });
    },
  },
};
</script>

<style scoped lang="scss"></style>
