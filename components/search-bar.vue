<template>
    <div class="searchBar_wrap">
        <div class="banner_wrap">
            <div class="search_title">
                <h1>Находите <span class="orange"> лучшие размещения</span> <br>по всей России!</h1>                
            </div>

            <div class="search_wrap">
                <div class="search_form">
                    <input id="city" type="text" placeholder="Город, регион, отель, аэропорт, вокзал или достопри...">
                    <input id="date" type="date" placeholder="dd/mm/yyyy">
                    <input type="text">
                    <button class="btn_prim">Найти</button>
                </div>
                <div class="seach_foot">
                    <p>Популярные направления:</p>
                </div>
                
                     
            </div>
           
            
        </div>
      
    </div>


</template>

<script>
export default {
   
}



</script>


<style scoped>


.search_title{
    width: 100%;
}

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

 h1{
    font-weight: 700;
    font-size: 48px;
    line-height: 50px;
    color: #0D0E20;
    
 }
 .orange{
    color: #FF5108
 }
.searchBar_wrap{
 display: flex;
 width: 100%;
 height: 556px;
 
}
.banner_wrap{
 display: flex;
 flex-direction: column;
 width: 100%;
 background-image: url("/banner.png");
 background-repeat: no-repeat;
 background-position: right 50%;
 justify-content: space-around;
align-items: center;
}



</style>