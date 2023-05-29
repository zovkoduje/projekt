<template>
    <swiper
    :slidesPerView="2"
    :spaceBetween="30"
    class="mySwiper"
    :breakpoints="{
      320: {
        slidesPerView: 1,
        spaceBetween: 10
      },
      750: {
        slidesPerView: 2,
        spaceBetween: 30
      }
    }"
  >
    <swiper-slide>
        <div class="flex items-center bg-white rounded-lg m-2 shadow-xl">
            <img class="h-32 m-5" src="/imgs/barchart.png">
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta quos ipsam, non nemo ipsum vel impedit excepturi asperiores magni earum eius nostrum exercitationem accusantium quam et ipsa nulla doloribus beatae?</p>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="flex items-center bg-white rounded-lg m-2 shadow-xl">
            <img class="h-32 m-5" src="/imgs/frame_103.png">
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta quos ipsam, non nemo ipsum vel impedit excepturi asperiores magni earum eius nostrum exercitationem accusantium quam et ipsa nulla doloribus beatae?</p>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="flex items-center bg-white rounded-lg m-2 shadow-xl">
            <img class="h-32 m-5" src="/imgs/group_33699.png">
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta quos ipsam, non nemo ipsum vel impedit excepturi asperiores magni earum eius nostrum exercitationem accusantium quam et ipsa nulla doloribus beatae?</p>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="flex items-center bg-white rounded-lg m-2 shadow-xl">
            <img class="h-32 m-5" src="/imgs/Round_chart.png">
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta quos ipsam, non nemo ipsum vel impedit excepturi asperiores magni earum eius nostrum exercitationem accusantium quam et ipsa nulla doloribus beatae?</p>
        </div>
    </swiper-slide>

    </swiper>
  </template>
  
  <script>

    import { Swiper, SwiperSlide } from 'swiper/vue';
    import 'swiper/css';
    import 'swiper/css/pagination';
    import 'swiper/css/autoplay';

    export default {
      components: {
        Swiper,
        SwiperSlide,
      },
      setup() {
        return {
          
        };
      },
    };
  </script>
  
  <style>
  </style>
  