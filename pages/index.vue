<template>
  <main>
    <div v-swiper:mySwiper1="swiperOption">
      <div class="swiper-wrapper">
        <div class="swiper-slide"><div class="text">Slide 1</div></div>
        <div class="swiper-slide"><div class="text">Slide 2</div></div>
        <div class="swiper-slide"><div class="text">Slide 3</div></div>
      </div>
      <div class="swiper-button-prev"></div>
      <div class="swiper-button-next"></div>
    </div>
    <div v-swiper:mySwiper2="swiperOption">
      <div class="swiper-wrapper">
        <div class="swiper-slide"><div class="text">Slide 4</div></div>
        <div class="swiper-slide"><div class="text">Slide 5</div></div>
        <div class="swiper-slide"><div class="text">Slide 6</div></div>
      </div>
      <div class="swiper-button-prev"></div>
      <div class="swiper-button-next"></div>
    </div>
  </main>
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
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
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
.swiper-container:first-of-type {
  background-color: rgba(128, 0, 0, 0.1);
}
.swiper-container:last-of-type {
  background-color: rgba(0, 0, 128, 0.1);
}
</style>
