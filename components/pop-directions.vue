<template>
    <div class="pop_dir_wrap">
        <h3 class="swipe_title" >Популярные направления</h3>
        <div class="swiper-button-next selectornx2" slot="button-next"></div>
        <div class="swiper-button-prev selectorpr2" slot="button-prev"></div>
       
        <swiper ref="mySwiper2" :options="swiperOptions" :modules="modules" class="swipers">
 
    
      <swiper-slide><img src="/sp.png" ></swiper-slide>
      <swiper-slide><img src="/altay.png" ></swiper-slide>
      <swiper-slide><img src="/camch.png" ></swiper-slide>
      <swiper-slide><img src="/baykal.png" ></swiper-slide>
      <swiper-slide><img src="/sp.png" ></swiper-slide>
      <swiper-slide><img src="/altay.png" ></swiper-slide>
      <swiper-slide><img src="/camch.png" ></swiper-slide>
      <swiper-slide><img src="/baykal.png" ></swiper-slide>
      
      
    </swiper>
    </div>
   
  </template>
   
  <script>
 import { Swiper, SwiperSlide } from 'vue-awesome-swiper';
 

    export default {
        components: {
        Swiper,
        SwiperSlide
    },
      data() {
        return {
          swiperOptions: {
            navigation: {
                nextEl: '.selectornx2',
                prevEl: '.selectorpr2'
                    },
            slidesPerView: 4,
            spaceBetween:30,
            keyboardControl: true,
           
          }
        }
      },
      computed: {
        swiper() {
            return this.$refs.mySwiper2.$swiper
          
        }
      },
      mounted() {
        console.log('Current Swiper instance object', this.swiper)
        this.swiper.slideTo(4, 1000, false)
      }
    }
  </script> 

<style scoped>

.swiper-button-next {
    top: 3.5%;
    left: 1760px !important;
    display: flex;
    right:10px;
    padding: 30px;
    background-image: url('/arr_r.png');
    color: transparent !important;
    fill: transparent !important;
    background-color: transparent !important;
    stroke: transparent !important;
    background-repeat: no-repeat;
    position: absolute

}
.swiper-button-prev {
    top: 3.5%;
    left: 1710px!important;
    width: 11px;
    height: 11px;
    display: flex;
    background-color: transparent !important;
    background-color: transparent !important;
    right:10px;
    padding: 30px;
    color: transparent !important;
    background-image: url('/arr_l.png');
    background-repeat: no-repeat;
   

}
    
.swipers img{
margin-top: 60px;
}
.pop_dir_wrap{
    width:100%;
    height: 400px;
    margin-top: 5%;
    position: relative
}


</style>