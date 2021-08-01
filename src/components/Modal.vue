<template>
    <div class="main">
        <div class="link-container">
            <div class="link">
                <div class="link-text">О нас</div>
                <img width="24" height="24" src="../assets/arrow.png" alt="">
            </div>
            <div class="link">
                <div class="link-text">Наша миссия</div>
                <img width="24" height="24" src="../assets/arrow.png" alt="">
            </div>
            <div class="link">
                <div class="link-text">Ooba Export</div>
                <img width="24" height="24" src="../assets/arrow.png" alt="">
            </div>
            <div class="link">
                <div class="link-text">Логистика</div>
                <img width="24" height="24" src="../assets/arrow.png" alt="">
            </div>

                             <v-select class="style-chooser" id="select-media" :options="langs" label="title">
    <template #option="{ title, src }">
    <div class="center s">
       <img :src="src"/><span style="margin: 0">{{ title }}</span>
    </div>
    </template>
  </v-select>

            <div style="margin-top:20px;" class="center icons">
                     <div class="icon-container center"><img src="../assets/I-1.png" alt=""></div>
                     <div class="icon-container center"><img src="../assets/i-2.png" alt=""></div>
                     <div class="icon-container center"><img src="../assets/i-3.png" alt=""></div>
                </div>

        </div>

    </div>
</template>

<script>
export default {
    props:['langs']
}
</script>

<style scoped>
#select-media{
    display: none;
    background: #fff;
}
.icons{
    width: 30%;
    justify-content: space-between;
    margin-left: 30%;
}
.link-text{
    font-family: Manrope;
font-style: normal;
font-weight: 500;
font-size: 24px;
line-height: 33px;
/* identical to box height */

font-feature-settings: 'liga' off;

color: #FFFFFF;
}
.main{
    position: fixed;
    width: 100%;
    min-height: 90vh;
    z-index: 10;
    backdrop-filter: blur(10px);
    top: 70px;
}
.link-container{
    background: #14142A;
    width: 100%;
    min-height: 50vh;
    padding: 0 0 30px 0;
}
.link{
    padding: 13px 5px;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    border-bottom: 1px solid #ccc;
}

@media screen and (max-width:695px) {
    #select-media{
        display: block;
    background: #fff;
    color:#fff;
}
}
</style>