<script setup lang="ts">
import swiper21 from '@/assets/images/banner-21.jpg'
import swiper22 from '@/assets/images/banner-22.jpg'
import swiper23 from '@/assets/images/banner-23.jpg'
import swiper24 from '@/assets/images/banner-24.jpg'

import { register } from 'swiper/element/bundle'

register()
</script>

<template>
    <swiper-container pagination="true" effect="coverflow" grab-cursor="true" centered-slides="true" slides-per-view="auto"
        coverflow-effect-rotate="50" coverflow-effect-stretch="0" coverflow-effect-depth="100" coverflow-effect-modifier="1"
        coverflow-effect-slide-shadows="true">
        <swiper-slide v-for="swiperImg in [
            swiper21,
            swiper22,
            swiper23,
            swiper24,
            swiper21,
            swiper22,
            swiper23,
            swiper24,

        ]" :key="swiperImg">
            <img :src="swiperImg" height="300" width="300" />
        </swiper-slide>
    </swiper-container>
</template>

<style lang="scss" scoped>
swiper-slide {
    background-position: center;
    background-size: cover;
    block-size: 300px;
    inline-size: 300px;
}
</style>
