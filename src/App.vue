<template>
  <div id="app">
    <BaseHeader/>
    <BaseMain/>
    <FooterTop/>
    <FooterMid/>
  </div>
</template>

<script>
import BaseHeader from './components/Header/BaseHeader'
import BaseMain from './components/Main/BaseMain'
import FooterTop from './components/Footer/FooterTop'
import FooterMid from './components/Footer/FooterMid.vue'

export default {
  name: 'App',
  components: {
    BaseHeader,
    BaseMain,
    FooterTop,
    FooterMid,
  }
}
</script>

<style lang="scss">
@import './assets/style/global.scss';
@import './assets/style/global.scss';
</style>
 