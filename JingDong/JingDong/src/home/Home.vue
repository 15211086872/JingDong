<template>
  <div class="home">
    <home-header></home-header>
    <home-anv></home-anv>
    <home-top></home-top>
    <home-mainstay></home-mainstay>
    <home-continue></home-continue>
    <home-boot></home-boot>
    
  </div>
</template>

<script>
import HomeHeader from './components/Header'
import HomeAnv from './components/Anv'
import HomeTop from './components/Top'
import HomeMainstay from './components/Mainstay'
import HomeContinue from './components/Continue'
import HomeBoot from './components/Boot'
export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomeAnv,
    HomeTop,
    HomeMainstay,
    HomeContinue,
    HomeBoot
  },
  data () {
    return {
      
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
