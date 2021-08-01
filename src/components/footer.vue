<template>
    <div class="main">
        <div class="main-container">

            <div class="support">

                 <div class="logo-container">
                     <div class="logo">
                         <img src="../assets/footer.png" alt="">
                     </div>
                 </div>

                 <div class="support-container">
                     <div class="support">
                          <div class="support-text">О нас</div>
                          <div class="support-text">Наша миссия</div>
                          <div class="support-text">Ooba Export</div>
                          <div class="support-text">Логистика</div>
                     </div>
                 </div>


                 <div class="icons-container">
                     <div class="icons">
                             <div class="icon">
                                 <img src="../assets/ins.png" alt="">
                             </div>

                             <div class="icon">
                                 <img src="../assets/facebook.png" alt="">
                             </div>

                             <div class="icon">
                                 <img src="../assets/tme.png" alt="">
                             </div>

                             <div class="icon">
                                 <img src="../assets/youtube.png" alt="">
                             </div>
                     </div>
                 </div>

            </div>

                 <div class="support-container-1">
                     <div>
                          <div class="support-text">О нас</div>
                          <div class="support-text">Наша миссия</div>
                          <div class="support-text">Ooba Export</div>
                          <div class="support-text">Логистика</div>
                     </div>
                 </div>


            <div class="line"></div>

           

           <div class="made-container">
               <div class="made">
                   Made by  <img class="wrap" src="../assets/footer1.png" alt=""> innnovat
               </div>
           </div>


        </div>
    </div>
</template>


<style scoped>
 .main{
        padding: 20px 0px 0px 5px;
    }
.support-text{
    padding: 10px;
    word-wrap: none;
    word-break: unset;
}
.support-container-1 div{
    display: flex;
    align-items: flex-start;
    justify-content: space-between;
}
.support-container-1{
    display: none;
    justify-items: flex-start;
    justify-self: flex-start;
    align-items: flex-start;
    align-self: flex-start;
    margin: 1px;
    padding: 5px;
}
.wrap{
    margin: 0px 5px 0px 10px;
    padding-top: 10px;
}
.made{
    font-family: Montserrat;
font-style: normal;
font-weight: 600;
font-size: 18px;
line-height: 22px;
/* identical to box height */


color: #FFFFFF;
}
.line{
    width: 100%;
    height: 1px;
    background: #FFFFFF;
opacity: 0.5;
margin: 30px 30px 30px 0px;
}
.icons-container{
 margin-left: 20px;
}
.icons{
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.icon{
    width: 32px;
    height: 32px;
    border-radius: 50%;
    background: rgba(0,0,0,.4);
margin: 0px 5px 0px 5px;
display: flex;
align-items: center;
justify-content: center;
}
.support-text{
    font-family: Manrope;
font-style: normal;
font-weight: 500;
font-size: 16px;
line-height: 22px;
/* identical to box height */

font-feature-settings: 'liga' off;

color: #FFFFFF;

}
.support{
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin: 0px 70px 0px 30px;
    width: 100%;
}
.main{
    background: #14142A;
    min-height: 30vh;
      display: flex;
    align-items: center;
    justify-content: center;
}
.main-container{
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 80%;
    height: 80%;
    flex-direction: column;
}

@media screen and (max-width:1150px) {
    .support-container{
        display: none;
        /* justify-self: flex-start; */
    }
    .support-container-1{
          display: flex;
    }
}
@media screen and (max-width: 390px) {
    .main-container{
        width: 90%;
    }
    .line{
        width: 50%;
    }
    .icon{
        margin: 0;
    }
   
}


</style>