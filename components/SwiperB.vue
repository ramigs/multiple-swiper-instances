<template>
  <div v-swiper:swiper="swiperOption">
    <div class="swiper-wrapper">
      <div class="swiper-slide"><div class="text">Slide 4</div></div>
      <div class="swiper-slide"><div class="text">Slide 5</div></div>
      <div class="swiper-slide"><div class="text">Slide 6</div></div>
    </div>
    <div class="swiper-button-prev"></div>
    <div class="swiper-button-next"></div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      swiperOption: {
        direction: 'horizontal',
        slidesPerView: 2,
        navigation: {
          nextEl: '.swiper-button-next',
          prevEl: '.swiper-button-prev'
        }
      }
    }
  }
}
</script>

<style lang="scss" scoped>
.swiper-container {
  width: 100%;
  height: 8rem;
  margin-bottom: 1em;
  background-color: rgba(0, 0, 0, 0.05);
}
.swiper-slide {
  font-family: sans-serif;
  text-align: center;
  font-size: 2em;
  line-height: 8rem;
}
</style>
