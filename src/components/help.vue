<template>
    <div class="main">
        <div class="left-pieces">
            <img src="../assets/kitay.png" alt="">
        </div>
        <div class="right-pieces center">
            <div class="container">
                <div class="text">
                    Мы поможем вам покорить рынок 
Китая!
                </div>
            </div>
        </div>
    </div>
</template>


<style scoped>
.main{
margin: 50px 0;
display: flex;
}
.left-pieces{
    width: 50%;
}
.right-pieces{
    background: url("../assets/wall.png") no-repeat,#F7FAFF;
    width: 150%;
    background-position: center right;

}
.container{
    width: 50%;

}
.container::before{
    content: "";
    display:inline-block;
    width: 5px;
    height: 200px;
    background: linear-gradient(180deg, #F29F05 0%, #F28705 31.25%, #F25C05 63.54%, #F20505 100%);
border-radius: 1.5px;
}
.text{
    font-family: Montserrat;
font-style: normal;
font-weight: bold;
font-size: 32px;
line-height: 46px;
    margin-top: -170px;
        margin-left: 18px;
/* or 144% */

font-feature-settings: 'liga' off;

/* 6 */

color: #14142A;

opacity: 0.95;
}


@media screen and (max-width:920px) {
    .main{
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }
    .left-pieces{
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;

}
.right-pieces{
    height: 500px;
width: 100%;
}
}

@media screen and (max-width:680px) {
    img{
        width: 90%;
    }
}

@media screen and (max-width:560px) {
    .container{
        width: 90%;
    }
}
</style>