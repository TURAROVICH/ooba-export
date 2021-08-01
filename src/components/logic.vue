<template>
    <div class="main center">
        <div class="main-container center">

            <div class="left center">
                <div class="title-container">
                    <div class="title">
Логистика сервиса
                    </div>
                </div>
                <div class="des-container">
                    <div class="des">
За транспортную логистику Ooba Export отвечает компания CAPS, располагающая почтовой лицензией.
                    </div>
                </div>
            </div>

            <div class="right">
              <img id="img" src="../assets/car.png" alt="">
            </div>

        </div>
    </div>
</template>


<style scoped>
.left{
    flex-direction: column;
    width: 30%;
    gap: 30px;
}
.main{
    width: 100%;
}
.main-conatiner{
    justify-content: space-between;
    width: 90%;
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
}


@media screen and (max-width:1125px) {
    .main{
        padding: 50px;
        margin: 0px 0px 0px 30px;
    }
}

@media screen and (max-width:1086px) {
    .main-container{
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
    }
    .left{
        width: 90%;
    }
    #img{
        width: 90%;
    }

}

@media screen and (max-width:504px) {
    .main{
        margin: 0;
    }
}
</style>