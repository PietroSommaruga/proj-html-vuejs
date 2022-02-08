<template>
  <div id="app">
    <header-section/>
    <main-Space/>
    <footer-content/>
  </div>
</template>

<script>
import headerSection from './components/headerSection.vue'
import mainSpace from './components/mainSpace.vue'
import footerContent from './components/footerContent.vue'

export default {
  name: 'App',
  components: {
    headerSection,
    mainSpace,
    footerContent
  }
}
</script>

<style lang="scss">
@import "./style/general.scss"; //scss generale -- Bootsrap -- Fontawesome
</style>
