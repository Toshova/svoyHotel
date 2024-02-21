<template>
    <div class="searchBar_wrap">
        <div class="banner_wrap">
            <h1>Находите <span class="orange"> лучшие размещения</span> <br>по всей России!</h1>
            <div class="search_wrap">
                <input id="city" type="text" placeholder="Город, регион, отель, аэропорт, вокзал или достопри...">
                <input type="text">
                <input type="text">
            <button class="btn_prim">Найти</button>
       </div>
        </div>
      
    </div>


</template>

<script>
export default {
   
}



</script>


<style scoped>
.search_wrap{
    display: flex;
    flex-direction: row;
    min-height: 160px;
    width: 80%;
    border: 1px solid red;
    margin-left: 100px;
    align-items: center;
    justify-content: space-around;
    background-color: white;
   
}
input{
    border: 1px solid #DCDFE2;
    height: 64px;
    width: 236px;

}
#city{
    width:40%;
    background-image: url("/geodata.png"); 
    background-repeat: no-repeat;
    background-position: 2% 50%;
    padding-left: 40px
}



 h1{
    font-weight: 700;
    font-size: 48px;
    line-height: 50px;
    color: #0D0E20;
    margin-left: 100px;
 }
 .orange{
    color: #FF5108
 }
.searchBar_wrap{
 display: flex;
 width: 100%;
 height: 556px;
 border: 1px solid red;
 
}
.banner_wrap{
 display: flex;
 flex-direction: column;
 width: 100%;
 background-image: url("/banner.png");
 background-repeat: no-repeat;
 background-position: right 50%;
 border: 1px solid rgb(0, 255, 123);
 justify-content: space-around;
}

.btn_prim{
    width: 184px;
    height: 64px;
    background-color: #FF5108;
    color: white;
}


</style>