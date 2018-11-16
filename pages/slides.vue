<template>
  <section >
    <swiper :options="swiperOption" ref="mySwiper" >
    <!-- slides -->
    <swiper-slide class="sw-1">I'm Slide 1</swiper-slide>
    <swiper-slide class="sw-1">I'm Slide 2</swiper-slide>
    <swiper-slide class="sw-1">I'm Slide 3</swiper-slide>
    <swiper-slide class="sw-1">I'm Slide 4</swiper-slide>
    <swiper-slide class="sw-1">I'm Slide 5</swiper-slide>
    <swiper-slide class="sw-1">I'm Slide 6</swiper-slide>
    <swiper-slide class="sw-1">I'm Slide 7</swiper-slide>
    <!-- Optional controls -->
    <div class="swiper-pagination"  slot="pagination"></div>
    <div class="swiper-button-prev" slot="button-prev"></div>
    <div class="swiper-button-next" slot="button-next"></div>
    <div class="swiper-scrollbar"   slot="scrollbar"></div>
  </swiper>
  </section>
</template>
<script>
  export default {
    name: 'carrousel',
    data() {
      return {
        swiperOption: {
          // some swiper options/callbacks
          // 所有的参数同 swiper 官方 api 参数
          // ...
        }
      }
    },
    computed: {
      swiper() {
        return this.$refs.mySwiper.swiper
      }
    }
  }
</script>
<style>
    .sw-1{
        height: 600px;
    }
</style>
