<template>
    <div class="main center">
        <div class="main-container center">
            <div class="text center">
                <div class="title-container center">
                <div class="title">
                    Реализуйте свою продукцию
на рынке Китая онлайн!
                </div>
                </div>
                
                <div class="des-container center">
                    <div class="des">
Мы предоставляем кыргызстанским предпринимателям возможность выхода на Китайский рынок!
                    </div>
                </div>
            </div>

            <!-- <div class="img-container center"> -->
                <!-- <div class="imgs center"> -->
                     <carousel-3d :autoplay="true" >
                             <slide :index="0">
                    <div class="center">
                    <img  src="../assets/bal.png" alt="">
                    </div>
                    </slide>
                        <slide :index="1">
                    <div class="center">
                    <img src="../assets/bal1.png" alt="">
                    </div>
                    </slide>
                        <slide :index="2">
                    <div class="center">
                    <img  src="../assets/bal2.png" alt="">
                    </div>
                    </slide>
                    </carousel-3d>
                <!-- </div> -->
            <!-- </div> -->

            <div class="imgs-description center">
                <div class="text-des center">
О вашем продукте узнают покупатели kитая и смогут его приобрести.
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import { Carousel3d, Slide } from 'vue-carousel-3d';
export default {
    components:{
           Carousel3d,
            Slide
    }
}
</script>
<style scoped>
.vs1__combobox{
    background: #fff;
}
.current,.left-1,.right-1{
    background: transparent;
    border:none;
}
.text-des{
font-family: Manrope;
font-style: normal;
font-weight: 800;
font-size: 32px;
line-height: 44px;
text-align: center;
font-feature-settings: 'liga' off;
}
.text{
    flex-direction: column;
    gap: 15px;
}
.imgs img{

    align-self: flex-end;
}
.imgs{
    overflow: hidden;
    gap: 10px;
}
.main{
    margin: 50px 0px 50px 0px;
}
.main-container{
    flex-direction: column;
    gap: 30px;
}
.title{
    font-style: normal;
font-weight: 800;
font-size: 38px;
line-height: 52px;
text-align: center;
text-transform: uppercase;
font-feature-settings: 'liga' off;

/* 4 */

color: #F20505;

}
.des{
    
font-family: Manrope;
font-style: normal;
font-weight: normal;
font-size: 20px;
line-height: 27px;
text-align: center;
font-feature-settings: 'liga' off;

/* 6 */

color: #14142A;

opacity: 0.8;
}


@media screen and (max-width:1090px) {
    .text{
        width: 80%;
    }
    .text-des{
        width: 70%;
        text-align: center;
    }
}

@media screen and (max-width:890px) {
    .text{
        width: 50%;
    }
    .text-des{
        width: 30%;
        text-align: center;
    }
    #i-1,#i-2{
        display: none;
    }
}


@media screen and (max-width:605px) {
    .text{
        width: 45%;
    }
    .text-des{
        width: 45%;
        text-align: center;
        font-size: 18px;
    }
    .title{
        font-size: 18px;
    }
}
</style>