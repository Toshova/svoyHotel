<template>
    <div class="best_imp_wrap">
        <h3 class="swipe_title" >Лучшие впечатления</h3>

        <div class="search_wrap">
                <div class="search_form">
                    <input id="city" type="text" placeholder="Город, регион, отель, аэропорт, вокзал или достопри...">
                    <input id="date" type="date" placeholder="dd/mm/yyyy">
                    <button class="btn_prim">Найти</button>
                </div>
                
                     
            </div>




        <div class="swiper-button-next selectornx3" slot="button-next"></div>
        <div class="swiper-button-prev selectorpr3" slot="button-prev"></div>
       
        <swiper ref="mySwiper3" :options="swiperOptions3" :modules="modules" class="swipers">
 
    
      <swiper-slide><img src="/church_1.png" ></swiper-slide>
      <swiper-slide><img src="/church_2.png" ></swiper-slide>
      <swiper-slide><img src="/church_3.png" ></swiper-slide>
      <swiper-slide><img src="/church_1.png" ></swiper-slide>
      <swiper-slide><img src="/church_2.png" ></swiper-slide>
      <swiper-slide><img src="/church_3.png" ></swiper-slide>
      
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
          swiperOptions3: {
           
            navigation: {
                        nextEl: '.selectornx3',
                        prevEl: '.selectorpr3'
                    },
            slidesPerView: 3,
            spaceBetween:20,
            keyboardControl: true,
           
          }
        }
      },
      computed: {
        swiper() {
            return this.$refs.mySwiper3.$swiper
          
        }
      },
      mounted() {
        console.log('Current Swiper instance object', this.swiper)
        this.swiper.slideTo(4, 1000, false)
      }
    }
  </script> 

<style scoped>


.search_form{
    width: 100%;
    display: flex;
    justify-content: space-between;
}


input{
    border: 1px solid #DCDFE2;
    height: 64px;
    width: 20%;

}
#city{
    width:45%;
    background-image: url("/geodata.png"); 
    background-repeat: no-repeat;
    background-position: 2% 50%;
    padding-left: 40px
}
 #date{
    width:35%;
 }

.swiper-button-next{
    top: 3%;
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
    top: 3%;
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
.best_imp_wrap{
    width:100%;
    min-height: 752px;
    position: relative;
    margin-top: 5%;
    display: flex;
    flex-direction: column;
    align-items: center;
}
.swipe_title {
    width: 100%;
    height: 40px;
    font-size: 38px;
    font-weight: 700;
    line-height: 40px;
}

</style>