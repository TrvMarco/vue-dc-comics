<template>
  <div id="app">
    <BaseHeader/>
    <BaseMain/>
    <FooterTop/>
  </div>
</template>

<script>
import BaseHeader from './components/Header/BaseHeader'
import BaseMain from './components/Main/BaseMain'
import FooterTop from './components/Footer/FooterTop'

export default {
  name: 'App',
  components: {
    BaseHeader,
    BaseMain,
    FooterTop
  }
}
</script>

<style lang="scss">
@import './assets/style/global.scss';
@import './assets/style/global.scss';
</style>
 