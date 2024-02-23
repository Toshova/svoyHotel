<template>
<div class="main_wrap">
  <searchBar/>
  <popDirections/>
  <bestAccom/>
  <div class="F1_wrap">
    <img src="/F1.png">
  </div>
  <bestImp/>
  <transFer/>
  <advIdeas/>
  <servLikes/>
  <footerMain/>
</div>
</template>

<script>
import searchBar from '../components/search-bar.vue';
import bestAccom from '../components/best-accom.vue';
import bestImp from '../components/best-imp.vue';
import transFer from '../components/trans-fer.vue';
import popDirections from '../components/pop-directions.vue';
import advIdeas from '../components/adv-ideas.vue';
import servLikes from '../components/serv-likes.vue';
import footerMain from '../components/footer-main.vue';


export default {
  name: 'IndexPage',

  components: {
    searchBar, 
    popDirections,
    bestAccom, 
    bestImp,
    transFer,
    advIdeas,
    servLikes,
    footerMain
  }
}
</script>
 <style>
.main_wrap {
  margin: 0 10%
}
.F1_wrap img {
  width:100%;
  height: auto;
  margin-top: 5%;
}
.btn_prim{
    width: 184px;
    height: 64px;
    background-color: #FF5108;
    color: white;
}
[type="date"]::-webkit-inner-spin-button {
  display: none;
}
[type="date"]::-webkit-calendar-picker-indicator {
  opacity: 0;
}

[type="date"] {
  background:#fff url('/arr_d.png')  97% 50% no-repeat ;
}

.search_wrap{
    width: 100%;
    height: 160px;
    display: flex;
    flex-direction: column;
    background-color: white;
    justify-content: center;
}

.swipe_title {
    width: 100%;
    height: 40px;
    font-size: 38px;
    font-weight: 700;
    line-height: 40px;
}

</style>