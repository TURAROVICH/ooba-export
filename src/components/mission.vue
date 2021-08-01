<template>
    <div class="main">
        <div class="main-container">
            <div class="flex">
                        <div class="text">
                            <div class="text-title">
                                <div class="title">
В чем основная миссия этого сервиса? 
                                </div>
                            </div>
                            <div class="text-des">
                                <div class="des">
                                    Электронная коммерция − это очень перспективная отрасль, оказывающая колоссальное влияние на мировую экономику. Поэтому, чтобы не отставать от успешных стран, где развит онлайн-шоппинг, и интегрироваться в систему международной электронной коммерции,мы создали платформу Ooba Export.  Этот сервис станет мощным рычагом развития экономики Кыргызстана.
                                </div>
                            </div>

                            <div class="text-button center">
                                <div class="button-text">
Узнать подробнее
                                </div>
                            </div>
                        </div>

                        <div class="img">
                            <img id="img" src="../assets/mission.png" alt="">
                        </div>
            </div>

        <why/>
            



        </div>
    </div>
</template>

<script>
import Why from './why-ooba'
export default {
    components:{
        Why
    }
}
</script>



<style scoped>
.flex{
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.text{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    gap: 30px;
}
.main{   
background: #F7FAFF;
padding: 50px 20px;
}
.text-button{
    width: 227px;
height: 60px;
border: 1px solid #F20505;
box-sizing: border-box;
border-radius: 50px;
}
.button-text{
    font-family: Manrope;
font-style: normal;
font-weight: 600;
font-size: 18px;
line-height: 28px;
/* identical to box height, or 156% */

display: flex;
align-items: center;
text-align: center;

/* 4 */

color: #F20505;
}
.title{
    font-family: Montserrat;
font-style: normal;
font-weight: bold;
font-size: 32px;
line-height: 39px;
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

@media screen and (max-width:1065px) {
    .flex{
        flex-direction: column-reverse;
    }
    #img{
        width: 100%;
    }
}
</style>