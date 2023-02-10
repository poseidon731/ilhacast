<template>
  <div id="myApp" >
    <nav-bar></nav-bar>
    <nuxt/>
    <Footer />
  </div>
</template>

<script>
import NavBar from '~/components/NavBar'
import Footer from '~/components/Footer'
export default {
  data () {
    return {

    }
  },
  components: { NavBar, Footer }
}
</script>

<style>
/* GLOBAL FONTS */
  @font-face {
    font-family: 'RobotoThin';
    src: url('~static/fonts/Roboto-Thin.ttf');
  }
  @font-face {
    font-family: 'OldeEnglish';
    src: url('~static/fonts/OldeEnglish.ttf');
  }

/* GLOBAL CSS CLASSES */
  * {
   margin: 0;
   padding: 0;
   font-family: RobotoThin;
  }
  
  html {
    scroll-behavior: smooth;
  }
  
  .container-shadow {
    box-shadow: 2px 1px 10px 2px;  /* x, y, smoth, strength */
    -webkit-backdrop-filter: blur(100px);
  }

  .container-flex {
    display: flex;
    flex-wrap: wrap; 
    flex-direction: row;
    width: 100%;
    padding: 0px 10px 10px 0px; 
    align-items: center;
    justify-content: center;
    box-sizing: border-box;

  }
  .container-item {
    flex: 1;
    text-align: center;
  }
  .align-right {
    text-align: right;
  }

  .align-left {
    text-align: left;
  }
  #myApp {
    background-image: url('/static/circuitos-eletricos.png');
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
  }
</style>

