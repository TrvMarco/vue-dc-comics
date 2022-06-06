<template>
  <div id="app">
    <BaseHeader/>
    <MainHero/>
    <CurrentSeries/>
    <FooterTop/>
    <FooterMid/>
    <FooterBottom/>
  </div>
</template>

<script>
import BaseHeader from './components/Header/BaseHeader'
import MainHero from './components/Main/MainHero'
import CurrentSeries from './components/Main/CurrentSeries.vue'
import FooterTop from './components/Footer/FooterTop'
import FooterMid from './components/Footer/FooterMid.vue'
import FooterBottom from './components/Footer/FooterBottom.vue'

export default {
  name: 'App',
  components: {
    BaseHeader,
    MainHero,
    CurrentSeries,
    FooterTop,
    FooterMid,
    FooterBottom,
  }
}
</script>

<style lang="scss">
@import './assets/style/global.scss';
</style>
 