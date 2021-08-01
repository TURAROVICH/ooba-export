<template>
    <div class="main center">
        <div class="main-conatiner">
             <div class="col">

                 <div class="about-1_container">

                     <div class="text-container center">
                         <div class="text">
                             <div class="title">Ooba Export</div>
                             <div class="des">
                                 Это платформа, предназначенная для удобной онлайн-продажи товаров от кыргызстанских производителей иностранным покупателям. Интуитивно понятный интерфейс и удобные фильтры поиска сделают сайт  максимально комфортным для пользователей.
                             </div>
                         </div>
                     </div>

 
                     <img id="about-1" src="../assets/img1.png" alt="">

                 </div>




                 <div class="about-2_container">

                     <div class="text-container center t-c">
                         <div class="text">
                             <div class="des">
                           Сервис расширит границы рынка сбыта для местных предпринимателей. В Кыргызстане много достойных производителей, которым давно пора выйти на международный рынок! Пока основным рынком сбыта мы выбрали Китай, так как там отлично развита электронная коммерция.
                             </div>
                         </div>
                     </div>

 
                     <img id="about-2" src="../assets/about2.png" alt="">

                 </div>


                 
                 
             </div>
        </div>
    </div>
</template>

<style scoped>
.t-c{
    width: 100%;
    height: 100%;
    padding: 50px;
}
#about-1,#about-2{
    width: 50%;

    /* width: 50%;/ */
}
.about-1_container{
    /* gap: 30px; */
    display: flex;
    align-items: center;
    justify-content: center;
background: #F7FAFF;

}
.about-2_container{
background: #F7FAFF;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: row-reverse;
}
.text-container{
    padding: 33.5px;
    height: 100%;
    width: 100%;
    background: #F7FAFF;
}
.text{
    width: 360px;
}
.title{
    font-family: Montserrat;
font-style: normal;
font-weight: 800;
font-size: 50px;
line-height: 61px;
/* identical to box height */

font-feature-settings: 'liga' off;

/* 6 */

color: #14142A;

opacity: 0.95;
}
.des{
    font-family: Manrope;
font-style: normal;
font-weight: normal;
font-size: 20px;
line-height: 32px;
/* or 160% */

font-feature-settings: 'liga' off;

/* 6 */

color: #14142A;

opacity: 0.8;


}


@media screen and (max-width:1125px) {
    #about-1,#about-2{
    width: 50%;

    /* width: 50%;/ */
}
#about-1{
    height: 120%;
}
}


@media screen and (max-width:820px) {
    .about-1_container,.about-2_container{
        flex-direction: column-reverse;
    }

     #about-1,#about-2{
    width: 100%;

    /* width: 50%;/ */
}
#about-1{
    height: 100%;
}


}


@media screen and (max-width:435px) {
    .title{
        font-size: 18px;
    }
    .text{
        width: 80%;
    }
}



</style>