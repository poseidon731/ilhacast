<template>
  <div class="index">
    <section class="section bg-white--invert">      
      <p class="section__title--sample">
        <a class="h1">Frase de efeito</a>
      </p>
      <br>
      <h4>algo sobre nós e do que falamos</h4>
      <h4>nosso mascote pode vir aqui</h4>
      
      <br>
      <!-- <h1>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nobis cumque error perferendis nostrum fugit fugiat nulla optio atque? Reprehenderit sequi aliquid minima nihil et esse deleniti, fugit aperiam ullam quisquam.</h1>     -->
    </section>
    <section class="section bg-white">
      <h1>Logos, um banner ou icones de tecnologias e parceiros talvez</h1>
      <br>
      <h3>Lorem ipsum dolor sit amet consectetur adipisicing elit.</h3>
  
    </section>
     <section id="hosts" class="section bg-white--invert">
       <div class="section__title">
        <h1>Hosts</h1>
       </div>
      <div class="section__hosts">
      <div class="host__avatar host__avatar--first" @click.native="alert('modal bacana (?)')">
        <p class="host__avatar__subtitle">Jhon</p>
      </div>
      <div class="host__avatar" @click.native="alert('modal bacana (?)')">
        <p class="host__avatar__subtitle">Doe</p>
      </div>
      <div class="host__avatar" @click.native="alert('modal bacana (?)')">
        <p class="host__avatar__subtitle">...</p>
      </div>
    </div>
    </section>
    
  </div>
</template>

<script>
import GirlCastBanner from '~/components/GirlCastBanner'

export default {
  components: {
    GirlCastBanner
  }
}
</script>

<style scoped>
.index {
  display: flex;
  flex-wrap: wrap;
  flex-direction: column;
  /* filter: invert(100%); */

}
.bg-gray {
  background-color: rgb(232, 231, 231);
}
.bg-white--invert {
  background: rgba(255, 255, 255, .9);
  filter: invert(100%);
}
.bg-white {
  background: rgba(255, 255, 255, 1);
  /* filter: invert(100%); */
}

.bg-sea {
  background: url('~static/bg.jpg');
  background-position: center;
  background-repeat: no-repeat; 
  background-size: cover;
  background-position-y: 0;
}
.bg-brain {
  background: url('~static/abstractbrain.png');
  background-position: center;
  background-repeat: no-repeat; 
  background-size: auto;
  
}
.bg-circuits {
  background: url('~static/circuitos-eletricos.png');
  background-position: center;
  background-repeat: no-repeat; 
  background-size: cover;
  color: azure;
  
}
.h1 {
  font-size: 24px;
  font-weight: bold;
}
.section {
  padding: 40px;
  flex: 1;
  display: flex;
  flex-direction: column; 
  justify-content: center;
  align-items: center;
  align-content: center;
  text-align: center;
  height: 250px;
  transition: .5s ease;
}
.section:hover {
  height: 300px;
}
.section--first {
  color: azure;
}
.section__title--sample a {
  text-decoration: none;
  /* color: black; */
}
.section__title {
  flex: 1;
  display: flex;
  align-items: center;
}
.section__hosts {
  padding-bottom: 30px; 
  height: 250px;
  flex: 1;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-content: center;
  align-items: center;
}
.host__avatar--first {
  margin-left: 0;
}
.host__avatar {
  margin: 20px;
  background: gray;
  width: 150px;
  height: 150px;
  border-radius: 50%;
  cursor: pointer;
  background: url('~static/Circuit-Man-Head.png');
  background-position: center;
  background-repeat: no-repeat; 
  background-size: contain;
  /* box-shadow: 1px 1px 5px tomato; */
}

.host__avatar__subtitle {
  position: relative;
  text-align: center;
  top: 70px;
}
</style>

