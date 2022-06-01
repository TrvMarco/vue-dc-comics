<template>
  <div id="app">
    <BaseHeader/>
    <BaseMain/>
    <FooterTop/>
    <FooterMid/>
    <FooterBottom/>
  </div>
</template>

<script>
import BaseHeader from './components/Header/BaseHeader'
import BaseMain from './components/Main/BaseMain'
import FooterTop from './components/Footer/FooterTop'
import FooterMid from './components/Footer/FooterMid.vue'
import FooterBottom from './components/Footer/FooterBottom.vue'

export default {
  name: 'App',
  components: {
    BaseHeader,
    BaseMain,
    FooterTop,
    FooterMid,
    FooterBottom
  }
}
</script>

<style lang="scss">
@import './assets/style/global.scss';
</style>
 