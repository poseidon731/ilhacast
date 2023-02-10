<template>
  <div class="container">
    <div class="text-container">
      <div>
        <h1>
          <slot></slot>
        </h1>
      </div>
    </div>
    <div class="girl-container" @mouseover="onGirlHover(true)" @mouseout="onGirlHover(false)">
      <img class="girl-colorful" src="~static/girl1.png" alt="">
      <img class="girl-pb" src="~static/girl0.png" alt="">
    </div>
    
  </div>
</template>

<script>
export default {
  data () {
    return {
      girlpb: null,
      girlcolorful: null
    }
  },
  methods : {
    onGirlHover (flag) {
      
      if (flag == true) {
        this.girlpb.style.opacity='0.7'
        this.girlcolorful.style.opacity='.3'
        return
      }
      
      this.girlpb.style.opacity='0.7'
      this.girlcolorful.style.opacity='0.3'
      
    }
  },
  mounted () {
    this.girlpb = document.querySelector('.girl-pb')
    this.girlcolorful = document.querySelector('.girl-colorful')
  }
}
</script>

<style scoped>
.container {
  padding-top: 20px;
  padding-bottom: 0px;
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  justify-content: center;
  height: 352px;
}

.text-container {
  /* background: rgba(108, 226, 252, 0.123); */
  text-align: center;
  flex: 1;
  display: flex;
  align-items: center;
  text-align: center;
}
.girl-container {
  position: absolute;
  opacity: 1;
  display: flex;
  justify-content: center;
  
  align-items: center;
  flex: 1;
}
  /* girl colorful */
.girl-container :nth-child(1) {
  width: 350px;
  opacity: 0.3;
  transition: 1s ease-in-out;
  
}

/* girl black and white */
.girl-container :nth-child(2) {
  position: absolute;
  width: 350px;
  opacity: .7;
  transition: 1s ease-in-out;
  /* filter: invert(100%); */
}

.girl-container :nth-child(2):hover {
  /* opacity: 1; */
}

</style>
