<template>
  <div id="app">
    <header-box :nav="nav"/>
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
  },
  data () {
    return {
      nav: [
        {
          id: 234235316,
          url: "#",
          label: "characters",
        },
        {
          id: 23454589,
          url: "#",
          label: "comics",
        },
        {
          id: 43534543,
          url: "#",
          label: "movies",
        },
        {
          id: 34543523,
          url: "#",
          label: "tv",
        },
        {
          id: 34534512,
          url: "#",
          label: "games",
        },
        {
          id: 34543545,
          url: "#",
          label: "collectibles",
        },
        {
          id: 36565623,
          url: "#",
          label: "videos",
        },
        {
          id: 56746745,
          url: "#",
          label: "fans",
        },
        {
          id: 45753445,
          url: "#",
          label: "news",
        },
        {
          id: 54623621,
          url: "#",
          label: "shop",
        }
      ]

    }
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');
@import './style/main.scss'
</style>
