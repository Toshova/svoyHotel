<template>
    <div class="trans_wrap">
        <div>
            <h3 class="swipe_title" >Трансфер из аэропортов,<br> вокзалов и отелей</h3>
        </div>
        <div>
            <h3>без посредников и переплат</h3>
        </div>
        <div class="group_wrap">
        <div class="img_wrap">
            <img src="/group.png" >
        </div>
        <div class="input_wrap">
                <div class="search_form">
                    <div class="input_l">
                        <input id="city" type="text" placeholder="Город, регион, отель, аэропорт, вокзал или достопри...">
                        <input id="date" type="date" placeholder="dd/mm/yyyy">
                    </div>
                    <div class="input_l">
                        <input id="city" type="text" placeholder="Город, регион, отель, аэропорт, вокзал или достопри...">
                    </div>
                    <div class="input_s">
                        <input type="text">
                    </div>
                    <div class="input_l">
                        <button class="btn_prim" id="btn_l">Найти</button>
                    </div>
                  
                </div>
           
        </div>


        </div>
        
    </div>
    
</template>

<script>


</script>

<style scoped>
.trans_wrap{
    width: 100%;
    min-height: 622px;
    margin-top: 5%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}
.swipe_title{
    height: 80px;
}
.group_wrap{
    height: 464px;
    display: flex;
    justify-content: space-around;
    align-items: flex-end;
}
.img_wrap{
width: 45%
}
.input_wrap{
width: 45%;

}
.search_form{
    width: 100%;
    min-height: 464px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}

input{
    border: 1px solid #DCDFE2;
    height: 64px;
    width: 100%;
}
.input_l{
    width: 100%
}
.input_s{
    width: 50%
}
#btn_l{
    width: 100%; 
}
</style>