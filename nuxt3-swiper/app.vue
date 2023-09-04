<template>
  <swiper
    :direction="'vertical'"
    :pagination="{
      clickable: true,
    }"
    :modules="modules"
  >
    <swiper-slide>Slide 1</swiper-slide>
    <swiper-slide>Slide 2</swiper-slide>
    <swiper-slide>Slide 3</swiper-slide>
    <swiper-slide>Slide 4</swiper-slide>
    <swiper-slide>Slide 5</swiper-slide>
    <swiper-slide>Slide 6</swiper-slide>
  </swiper>
</template>

<script>
  // 导入 Swiper、SwiperSlide 组件
  import { Swiper, SwiperSlide } from 'swiper/vue';
  // 导入 Swiper 基础样式
  import 'swiper/css';
  // 导入 Pagination 模块样式
  import 'swiper/css/pagination';
  // 导入 Pagination 模块
  import { Pagination } from 'swiper/modules';

  export default {
    components: {
      Swiper,
      SwiperSlide
    },
    setup() {
      return {
        modules: [Pagination]
      };
    }
  };
</script>

<style>
#__nuxt {
  height: 100%;
}

html,
body {
  position: relative;
  height: 100%;
}

body {
  background: #eee;
  font-family: Helvetica Neue, Helvetica, Arial, sans-serif;
  font-size: 30px;
  color: #000;
  margin: 0;
  padding: 0;
}

.swiper {
  width: 100%;
  height: 100%;
  /* width: 500px;
  height: 500px; */
  border: 1px solid red;
}
</style>