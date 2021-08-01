<template>
  <div id="app">
    <Nav/>
    <Welcome/>
    <about-export/>
    <Gordost/>
        <Mission/>
        <Logic/>
        <Help/>
    <HelloWorld/>
  </div>
</template>

<script>
import Nav from './components/header'
import HelloWorld from './components/footer.vue'
import Welcome from './components/welcome'
import AboutExport from './components/about-export'
import Gordost from './components/gordost'
import Mission from './components/mission'
import Logic from './components/logic'
import Help from './components/help'
export default {
  name: 'App',
  components: {
    HelloWorld,
    Nav,
    Welcome,
    AboutExport,
    Gordost,
    Mission,
    Logic,
    Help
  }
}
</script>

<style>
.center{
  display: flex;
  align-items:center;
  justify-content: center
}
  @import url('https://fonts.googleapis.com/css2?family=Manrope:wght@300&display=swap');
  @import url('https://fonts.googleapis.com/css2?family=Manrope:wght@300&family=Montserrat&display=swap');
  *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family:Manrope ;
  }
  html,body{
    overflow-x: hidden;
  }
</style>
