<script>
import Header from '../src/components/Header/Header.vue'
import Promo from '../src/components/Promo/Promo.vue'
import AboutMe from '../src/components/AboutMe/AboutMe.vue'
import Portfolio from '../src/components/Portfolio/Portfolio.vue'

export default {
  name: 'App',
  components: {
    Header,
    Promo,
    AboutMe,
    Portfolio
  }
}
</script>


<template>
  <Header></Header>
  <Promo></Promo>
  <AboutMe></AboutMe>
  <Portfolio></Portfolio>
</template>



<style>
@import url(./assets/fonts/fonts.css);
#app {
  margin: 0;
  padding: 0;
  font-family: Inter, Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #FFF;
  background-color: #202020;
}
</style>
