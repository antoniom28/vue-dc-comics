<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Main from './components/Main.vue'
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Main,
    Header,
    Footer,
  },
}
</script>
<style>
  @import "./assets/style/global.scss";
  #app{
    min-width: 1200px;
  }
</style>
