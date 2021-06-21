<template>
  <div id="app">
    <Header :links="this.links_menu" />
    <Main />
    <Footer :links="this.links_menu" />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  },
  data () {
    return {
      links_menu: [
        {
          testo: "home",
          link: "/",
          active: true
        },
        {
          testo: "shop",
          link: "/",
          active: false
        },
        {
          testo: "about",
          link: "/",
          active: false
        },
        {
          testo: "gallery",
          link: "/",
          active: false
        },
        {
          testo: "locations",
          link: "/",
          active: false
        },
        {
          testo: "journal",
          link: "/",
          active: false
        },
        {
          testo: "contact",
          link: "/",
          active: false
        },
        {
          testo: "my account",
          link: "/",
          active: false
        }
      ]
    }
  }
}
</script>

<style lang="scss">
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
</style>
