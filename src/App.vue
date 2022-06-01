<template>
  <div id="app">
    <BaseHeader/>
    <BaseMain/>
  </div>
</template>

<script>
import BaseHeader from './components/Header/BaseHeader'
import BaseMain from './components/Main/BaseMain'

export default {
  name: 'App',
  components: {
    BaseHeader,
    BaseMain
  }
}
</script>

<style lang="scss">
@import './assets/style/global.scss';
</style>
 