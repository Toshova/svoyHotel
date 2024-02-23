<template>
    <div class="nav_wrap">
        <div class="label">
            <div >
                <svg width="33" height="24" viewBox="0 0 33 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M1.3922 9.50217C1.43848 8.14533 2.40447 6.98979 3.74418 6.68879L29.9568 0.799313C32.2941 0.274157 33.6528 3.31821 31.6844 4.6697L4.40476 23.3994C2.93122 24.4111 0.92086 23.3294 0.981312 21.5575L1.3922 9.50217Z" fill="#FF5108"/>
</svg>
            <svg width="34" height="23" viewBox="0 0 34 23" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M32.6957 15.455C32.5673 16.8186 31.5173 17.9215 30.1477 18.1313L2.52199 22.3621C0.164441 22.7231 -0.983465 19.6177 1.05465 18.3923L30.5947 0.630765C32.1261 -0.290058 34.0652 0.90725 33.8992 2.67101L32.6957 15.455Z" fill="#FF5108"/>
</svg>

        </div>
<p>SVOY HOTEL</p>
        </div>

        <div class="icons_center">
            <div class="icon">
                <img src="/home.png" >
                <p >Размещения</p>
            </div>
            <div class="icon">
                <img src="/church.png">
                <p >Впечатления</p> 
                </div>
            <div class="icon">
                <img src="/car.png">
                <p >Трансфер</p>
            </div>
            <div class="icon">
                <img src="/two_people.png">
                <p> Мероприятия</p>
            </div>
        </div>
       
<div class="icons_right">
    <img src="/help.png">
    <img src="/lang.png">
<button class="btn_base">Войти</button>
</div>
    </div>
</template>

<script>
export default{

}

</script>

<style>
.nav_wrap{
    display: flex;
    width: 100%;
    height: 72px;
    align-items: center;
    justify-content: space-around;
}
.label{
    display: flex;
    width: 142px;
    height: 40px;
    align-items: center;
    justify-content: space-between;
    color: #0D0E20;
    font-weight: 900;
    font-size: 15px;

}

.icons_center{
    display: flex;
    align-items: center;
    width: 578px;
    justify-content: space-between;
}
.icons_right{
    display: flex;
    align-items: center;
    width: 208px;
    justify-content: space-between;
}
.icon{
    display: flex; 
    width: 140px; 
    align-items: center;
    font-size: 14px;
    font-weight: 600;
    line-height: 20px;
}

.icon img{
    width: 16px;
    height: 14px;
}
.icon p{
    margin-left: 10px;
}


.btn_base{
    width: 104px;
    height: 40px;
    border: solid 1px #FF5108;
    color:#FF5108;
    font-weight: 600;
}
</style>