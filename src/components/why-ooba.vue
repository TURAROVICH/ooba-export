<template>
    <div class="main center">
        <div class="main-container center">
            <div class="title-container center">
                <div class="title">Почему Ooba Export нужен стране? </div>
            </div>

            <div class="cards">

                <div class="card center">
                     <img src="../assets/card.png" alt="">

                     <div class="des-container center">
                         <div class="des">
Сервис будет способствовать повышению экспорта продукции, производимой местными компаниями и индивидуальными предпринимателями
                         </div>
                     </div>
                </div>

                <div class="card center">
                     <img src="../assets/card1.png" alt="">

                     <div class="des-container center">
                         <div class="des">
Мы предоставляем платформу, где каждый желающий сможет онлайн реализовывать свой товарна китайском рынке!
                     </div>
                </div>
            </div>

                 <div class="card center">
                     <img src="../assets/card1.png" alt="">

                     <div class="des-container center">
                         <div class="des">
Экономика Кыргызстана начнет интенсивно развиваться </div>
                </div>
                 </div>



                 <div class="card center">
                     <img src="../assets/card1.png" alt="">

                     <div class="des-container center">
                         <div class="des">
Электронная коммерция в стране поднимется на совершенно новый уровень!
                    </div>
                    </div>
                 </div>

 </div>
                 </div>
        </div>
</template>


<style scoped>
.main-container,.card{
    flex-direction: column;
}
.cards{
    display: flex;
    align-items: flex-start;
    justify-content: space-evenly;
    flex-wrap: nowrap;
    margin: 10px 0;
        gap:0;
}
.card{
    width: 30%;
    margin: 30px 0;
    }
.des{
    font-family: Manrope;
font-style: normal;
font-weight: normal;
font-size: 20px;
line-height: 32px;
/* or 160% */

text-align: center;
font-feature-settings: 'liga' off;

/* 6 */

color: #14142A;

opacity: 0.8;
}
.title{
    font-family: Montserrat;
font-style: normal;
font-weight: bold;
font-size: 32px;
line-height: 39px;
/* identical to box height */

font-feature-settings: 'liga' off;

/* 6 */

color: #14142A;
}
@media screen and (max-width:960px) {
    .card{
        width: 200px;
    }
    .cards{
        flex-wrap: wrap;
    }
}


@media screen and (max-width: 545px) {
    .card{
        flex-direction: row;
        margin: 30px 0;
        width: 100%;
        margin-left: -50px;
    }
}

@media screen and (max-width:410px) {
    .title{
        font-size: 18px;
    }
    .title-container{
        width: 70%;
    }
    .card{
        flex-direction: column;
    }
    
}
</style>