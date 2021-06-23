<template>
  <div id="app">
    <Header :links="this.links_menu_header" />
    <Main />
    <Footer :links="this.links_menu_footer" />
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
      links_menu_header: [
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
      ],
      links_menu_footer: [
        {
          testo: "shop",
          link: "/"
        },
        {
          testo: "about",
          link: "/"
        },
        {
          testo: "gallery",
          link: "/"
        },
        {
          testo: "locations",
          link: "/"
        },
        {
          testo: "journal",
          link: "/"
        },
        {
          testo: "contact",
          link: "/"
        },
        {
          testo: "orders",
          link: "/"
        }
      ]
    }
  }
}
</script>

<style lang="scss">
@import '~@fortawesome/fontawesome-free/css/all.min.css';
@import '~bootstrap/dist/css/bootstrap.css';

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
</style>
