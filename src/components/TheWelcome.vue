<script setup lang="ts">
import swiper21 from '@/assets/images/banner-21.jpg'
import swiper22 from '@/assets/images/banner-22.jpg'
import swiper23 from '@/assets/images/banner-23.jpg'
import swiper24 from '@/assets/images/banner-24.jpg'
import { register } from 'swiper/element/bundle'

register()
</script>

<template>
  <div class="swiper-box">
    <swiper-container pagination="true" centered-slides="true" effect="cube" grab-cursor="true" cube-effect-shadow="true"
      cube-effect-slide-shadows="true" cube-effect-shadow-scale="0.94">
      <swiper-slide v-for="swiperImg in [
        swiper21,
        swiper24,
        swiper22,
        swiper23,
      ]" :key="swiperImg">
        <img :src="swiperImg" height="300" width="300" />
      </swiper-slide>
    </swiper-container>

    <swiper-container pagination="true" centered-slides="true" effect="cube" grab-cursor="true" cube-effect-shadow="true"
      cube-effect-slide-shadows="true" cube-effect-shadow-scale="0.94">
      <swiper-slide v-for="swiperImg in [
        swiper21,
        swiper24,
        swiper22,
        swiper23,
      ]" :key="swiperImg">
        <img :src="swiperImg" height="300" width="300" />
      </swiper-slide>
    </swiper-container>
  </div>
</template>

<style lang="scss" scoped>
swiper-slide {
  background-position: center;
  background-size: cover;
  block-size: 300px;
  inline-size: 300px;
}

swiper-container {
  margin: auto;
  block-size: 300px;
  inline-size: 300px;
}

.swiper-box {
  margin-block: 200px;
  display: flex;
  justify-content: space-around;
}
</style>