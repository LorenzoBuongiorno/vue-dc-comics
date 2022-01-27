<template>
  <div id="app">
    <header-box/>
    <jumbotron/>
  </div>
</template>

<script>
import HeaderBox from './components/HeaderBox.vue'
import Jumbotron from './components/Jumbotron.vue'

export default {
  name: 'App',
  components: {
    HeaderBox,
    Jumbotron
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');
@import './style/main.scss'
</style>
