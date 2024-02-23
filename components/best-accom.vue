<template>
    <div class="best_acc_wrap">
        <h3 class="swipe_title" >Лучшие размещения</h3>
        <div class="swiper-button-next selectornx1" slot="button-next"></div>
        <div class="swiper-button-prev selectorpr1" slot="button-prev"></div>
       
        <swiper ref="mySwiper1" :options="swiperOptions1" :modules="modules" class="swipers">
 
    
      <swiper-slide><img src="/acc_1.png" ></swiper-slide>
      <swiper-slide><img src="/acc_2.png" ></swiper-slide>
      <swiper-slide><img src="/acc_3.png" ></swiper-slide>
      <swiper-slide><img src="/acc_1.png" ></swiper-slide>
      <swiper-slide><img src="/acc_2.png" ></swiper-slide>
      <swiper-slide><img src="/acc_3.png" ></swiper-slide>
      
      
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
          swiperOptions1: {
           
            navigation: {
                        nextEl: '.selectornx1',
                        prevEl: '.selectorpr1'
                    },
            slidesPerView: 3,
            spaceBetween:30,
            keyboardControl: true,
           
          }
        }
      },
      computed: {
        swiper() {
            return this.$refs.mySwiper1.$swiper
          
        }
      },
      mounted() {
        console.log('Current Swiper instance object', this.swiper)
        this.swiper.slideTo(4, 1000, false)
      }
    }
  </script> 

<style scoped>

.swiper-button-next{
  top: 3.5%;
    left: 1760px !important;
    display: flex;
    right:10px;
    padding: 30px;
    background-image: url('/arr_r.png');
    color: transparent !important;
    fill: transparent !important;
    background-color: transparent !important;
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
.best_acc_wrap{
    width:100%;
    height: 648px;
    position: relative;
}
.swipe_title {
    width: 100%;
    height: 40px;
    font-size: 38px;
    font-weight: 700;
    line-height: 40px;
}

</style>