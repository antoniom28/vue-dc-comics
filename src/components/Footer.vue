<template>
  <footer>
    <div class="container">
      <footerBuyMenu />
      <footerCenter />
      <footerLastBar />
    </div>
  </footer>
</template>

<script>
import footerBuyMenu from './footerBuyMenu.vue'
import footerCenter from './footerCenter.vue'
import footerLastBar from './footerLastBar.vue'

export default {
  name: 'Footer',
  components:{
  footerBuyMenu,
  footerCenter,
  footerLastBar,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>

</style>
