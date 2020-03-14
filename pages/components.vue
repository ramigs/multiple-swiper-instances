<template>
  <main>
    <SwiperA />
    <SwiperB />
  </main>
</template>

<script>
import SwiperA from '../components/SwiperA.vue'
import SwiperB from '../components/SwiperB.vue'
export default {
  components: {
    SwiperA,
    SwiperB
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
.swiper-container:first-of-type {
  background-color: rgba(128, 0, 0, 0.1);
}
.swiper-container:last-of-type {
  background-color: rgba(0, 0, 128, 0.1);
}
</style>
