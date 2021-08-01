<template>
    <div :class="{bg:isModal}" class="main center ">
        <div class="left center">
            <div class="burger-container center">
                <div @click="isModal=!isModal" class="burgers">
                    <div :class="{to:isModal,color:isModal}" class="burger"></div>
                    <div :class="{color:isModal}"  class="main-burger"></div>
                    <div :class="{to:isModal,color:isModal}" class="burger"></div>
                </div>
            </div>
            <div class="logo-container center">
                <div class="logo">
                    <img v-if="!isModal" src="../assets/logo-mqin.png" alt="" class="logo">
                    <img v-else src="../assets/ooba.png" class="logo">
                </div>
            </div>
            <div class="nav-container center">
                <div class="nav">
                    <div class="nav-link">О нас</div>
                    <div class="nav-link">Наша миссия</div>
                    <div class="nav-link">Ooba Export</div>
                    <div class="nav-link">Логистика</div>
                </div>
            </div>
        </div>

        <div class="right center">
            <div class="center select-container">
                  <v-select id="select" :options="langs" label="title">
    <template #option="{ title, src }">
    <div class="center s">
       <img :src="src"/><span style="margin: 0">{{ title }}</span>
    </div>
    </template>
  </v-select>
            </div>
            <div class="center icons-container center">
                <div class="center icons">
                     <div class="icon-container center"><img src="../assets/Instagram.png" alt=""></div>
                     <div class="icon-container center"><img src="../assets/Twitter.png" alt=""></div>
                     <div class="icon-container center"><img src="../assets/Youtube1.png" alt=""></div>
                </div>
            </div>

            <div class="button-container center">
                <div class="button center">
                    <div class="button-text">
Перейти на сайт
                    </div>
                </div>
            </div>
        </div>
<transition name="slide-fade">
<Modal :langs="langs" v-if="isModal"/>
</transition>


    </div>
</template>

<script>
import vSelect from 'vue-select'
import Modal from './Modal'
export default {
    data:()=>({
      isModal:false,
      langs: [
      {
        title: "RU",
        src :'rul.png'
      },
       {
        title: "EN",
        src :'en.png'
      },
       {
        title: "CH",
        src :'ch.png'
      }
    ]
    }),
    components:{
        vSelect,
        Modal
    }
}
</script>


<style scoped>
#select{
    background: #fff;
}
.color{
    background-color: rgb(255,255,255);
}
.bg{
   background: rgba(20, 20, 42, 1);
}
.to{
    align-self: flex-end;
}

.slide-fade-enter-active {
  transition: all .3s ease;
}
.slide-fade-leave-active {
  transition: all .8s cubic-bezier(1.0, 0.5, 0.8, 1.0);
}
.slide-fade-enter, .slide-fade-leave-to
/* .slide-fade-leave-active до версии 2.1.8 */ {
  transform: translateX(100px);
  opacity: 0;
}


.burger-container{
    display: none;
}
.burgers{
    display: flex;
    align-items: flex-start;
    justify-content: flex-start;
    flex-direction: column;
    gap: 5px;
    margin: 0px 0px 0px 20px;
}
.burger{
    width: 25px;
    height: 4px;
    border-radius: 15px;
    background: rgba(20, 20, 42, 1);
}
.main-burger{
    width: 35px;
    height: 5px;
    background: rgba(20, 20, 42, 1);
    border-radius: 15px;
}
.s{
    justify-content: space-around;
}
.left{
    gap: 30px;
}
.right{
    justify-content: flex-end;
    gap: 30px;
}
.icons{
    gap: 30px;
}
  .nav{
      display: flex;
      align-items: center;
      justify-content: flex-start;
      gap: 10px;
  }
.main{
    border-bottom: 1px solid #ccc;
    justify-content: space-between;
    max-height: 70px;
    width: 100%;
}
.button{
background: #F20505;
width: 229px;
height: 70px;
}
.button-text{
    font-family: Manrope;
font-style: normal;
font-weight: 600;
font-size: 16px;
line-height: 28px;
/* identical to box height, or 175% */

display: flex;
align-items: center;
text-align: center;

color: #FFFFFF;
}

.nav{
    font-family: Manrope;
font-style: normal;
font-weight: 500;
font-size: 16px;
line-height: 22px;
/* identical to box height */

font-feature-settings: 'liga' off;

/* 6 */

color: #14142A;
}

@media screen and (max-width:1150px) {
    .select-container{
        display: none;
    }
}

@media screen and (max-width:1050px) {
    .select-container{
        display: block;
    }
    .icons-container{
        display: none;
    }
    .nav-container{
        display: none;
    }
    .burger-container{

        display: block;
    }
}


@media screen and (max-width:695px) {
    #select{
        display: none;
    }
}

@media screen and (max-width:550px) {
    .button{
background: #F20505;
width: 190px;
height: 70px;
}
}


@media screen and (max-width:500px) {
    .button{
background: #F20505;
width: 170px;
height: 70px;
}
}


@media screen and (max-width:400px) {
        .button{
background: #F20505;
width: 130px;
height: 70px;
}
.button-text{
    font-size: 12px;
}
.burgers{
    margin: 0;
}
.logo-container{
    margin-left: -30px;
}
}
</style>