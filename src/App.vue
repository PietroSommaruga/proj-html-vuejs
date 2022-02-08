<template>
  <div id="app">
    <header-section/>
    <main-first/>
    <main-second/>
    <main-third/>
    <footer-content/>
  </div>
</template>

<script>
import headerSection from './components/headerSection.vue'
import mainFirst from './components/mainFirst.vue'
import mainSecond from './components/mainSecond.vue'
import mainThird from './components/mainThird.vue'
import footerContent from './components/footerContent.vue'

export default {
  name: 'App',
  components: {
    headerSection,
    mainFirst,
    mainSecond,
    mainThird,
    footerContent
  }
}
</script>

<style lang="scss">
@import "./style/general.scss"; //scss generale -- Bootsrap -- Fontawesome
</style>
