<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />


    <testOggi v-for="(item,index) in testo" :key="index" 
    :scrivi="item.name +'-->String'" :scrivi-item="item"/>
  </div>
</template>

<script>
import Main from './components/Main.vue'
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import testOggi from './components/testOggi.vue'

export default {
  name: 'App',
  components: {
    Main,
    Header,
    Footer,
    testOggi, /* da togliere */
  },
  data(){
    return{
      testo : [
        {
          name : 'pep'
        },
        {
          name : 'cia'
        },
        {
          name : 'pasta'
        },
      ],
    }
  },
}
</script>
<style>
  @import "./assets/style/global.scss";
  #app{
    min-width: 1200px;
  }
</style>
