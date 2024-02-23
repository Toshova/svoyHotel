<template>
    <div class="serv_wrap">
        <div class="serv_card">
            <div class="card_wrap">
                <img src="/like.png" alt="">
                <h1>Индивидуальный подход</h1>
                <p>Нам важны индивидуальные <br>пожелания каждого</p>
            </div>  
        </div>

        <div class="serv_card">
             <div class="card_wrap">
                <img src="/like.png" alt="">
                <h1>Без посредников</h1>
                <p>Прямой доступ к ценам и специальным<br> предложениям</p>
            </div>
        </div>
        <div class="serv_card">
            <div class="card_wrap">
                <img src="/like.png" alt="">
                <h1>Онлайн 24/7</h1>
                <p>Наша служба поддержки на связи <br>круглосуточно</p>
            </div>
        </div>
    </div>
</template>
<script>
export default{

}
</script>

<style scoped>
.serv_wrap{
    display: flex;
    width: 100%;
    min-height: 336px;
    background-color: #F4F5F6;
    margin-top: 5%;
    justify-content: space-around;
    align-items: center;
}
.serv_card{
    width:30%;
    min-height: 208px;
    background-color: white;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
}
.serv_card h1{
    color: #0D0E20;
    font-size:24px;
    font-weight: 600;
    line-height:28px;
}
.serv_card p{
    color: #838A90;
    font-size:16px;
    font-weight: 400;
    line-height:24px;
}
.serv_card img{
    width:56px;
    height:56px;
}
.card_wrap{
    width: 90%;
    min-height: 208px;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
}
</style>