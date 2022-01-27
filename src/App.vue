<template>
  <div id="app">
    <header-box/>
    <jumbotron-box/>
    <footer-box/>
  </div>
</template>

<script>
import HeaderBox from './components/HeaderBox.vue'
import JumbotronBox from './components/JumbotronBox.vue'
import FooterBox from './components/FooterBox.vue'

export default {
  name: 'App',
  components: {
    HeaderBox,
    JumbotronBox,
    FooterBox
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');
@import './style/main.scss'
</style>
