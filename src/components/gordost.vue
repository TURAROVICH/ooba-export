<template>
    <div class="main center">
        <div class="main-container center">
                        <div class="text">
                                    <div class="text-title">
                                        <div class="title">Нам есть чем гордиться.</div>
                                    </div>
                                    <div class="text-des">
                                        <div class="des">
                                            Ooba Export раскроет весь потенциал страны.
                                        </div>
                                    </div>
                        </div>

                        <img id="img" src="../assets/map.png" alt="">
        </div>
    </div>
</template>


<style scoped>

.main{
    padding: 30px 50px;
}
.main-container{
    width: 80%;
    gap: 30px;
}
.title{
    font-family: Montserrat;
font-style: normal;
font-weight: 800;
font-size: 50px;
line-height: 61px;
font-feature-settings: 'liga' off;

/* 6 */

color: #14142A;
}

.des{
    font-family: Manrope;
font-style: normal;
font-weight: normal;
font-size: 20px;
line-height: 32px;
/* identical to box height, or 160% */

font-feature-settings: 'liga' off;

/* 6 */

color: #14142A;

opacity: 0.8;
}

@media screen and (max-width: 1100px) {
 .main-container{
     flex-direction: column;
 }   
 #img{
     width: 100%;
 }
}

@media screen and (max-width:380px) {
    .title{
        font-size: 18px;

    }
    .text{
        width: 90%;
    }
}
</style>