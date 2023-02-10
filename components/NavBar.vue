<template>
  <div class="container-flex">
    <div class="container-item">
      <p>O melhor, mais top e mais pica ! </p>
    </div>
    <div class="container-item">
      <logo name="ilhacast" />
    </div>

    <div class="container-item">
      <div class="">
        <a href="https://github.com/topdevs/ilhacast">
          <i class="fa fa-github-alt"></i>
          Github
        </a>
      </div>
    </div>
  </div>
</template>
<style lang="scss" scoped>
  .container-flex {
    padding-top: 10px;
    padding-bottom: 15px;
    color: azure;
    background-color: rgba(15, 15, 15 , 1);
  }

  a {
    text-decoration: none;  
    color: azure;
  }
</style>


<script>
import logo from '~/components/Logo'
export default {
  components: {
    logo
  },
  data () {
    return {

    }
  },// end data

  mounted () {

  } // end mounted
}
</script>
