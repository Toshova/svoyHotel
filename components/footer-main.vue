<template>
    <div class="foot_wrap">
        <div class="foot_stripe">
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
            <button>О компании</button>
            <button>Сотрудничество</button>
            <button>Идеи для путешествий</button>
            <button>Помощь (FAQ)</button>
            <button>Вакансии</button>
            <button>Контакты</button>
        </div>

        <div class="foot_stripe">
            <div class="contacts">
                <div class="contact">
                <div class="city">
                    <img src="/location.png">
                    <p>Санкт-Петербург</p>
                </div>        
                <p class="tel_num">+7 812 334 99 92</p>
            </div>
            <div class="contact">
                <div class="city">
                    <img src="/location.png">
                    <p>Москва</p>
                </div>        
                <p class="tel_num">+7 495 989 80 30</p>
            </div>
            <div class="contact">
                <div class="city">
                    <img src="/location.png">
                    <p>Сочи</p>
                </div>        
                <p class="tel_num">+7 938 470 07 37</p>
            </div>
            <div class="contact">
               <p class="city">Info@svoy-hotel.ru</p>
            </div>
            </div>
            <div class="icons">

            </div>
            
        </div>

       
    </div>
</template>
<script>

</script>

<style scoped>

.icons{
    display: flex;
    width: 40%;
    border: 1px solid purple;
}
.contacts{
    display: flex;
    width: 55%;
    border: 1px solid purple;
    justify-content: space-between;
}
.contact{
    display: flex;
    flex-direction: column;
}

.contact img{
    width: 16px;
    height: 16px;
}
.foot_wrap{
    width: 100%;
    min-height: 270px;
    display: flex;
    flex-direction: column;
    margin-top: 5%;
}
.foot_stripe{
    width: 100%;
    display: flex;
    justify-content: space-around;  
}
button{
    
    font-size: 16px;
    font-weight: 600;
    line-height: 20px;
}
.city{
    display: flex;
    font-size: 16px;
    font-weight: 600;
    line-height: 20px;
    color: #0D0E20;
}
.tel_num{
    font-size: 14px;
    font-weight: 400;
    color: #838A90;
}
</style>