<template>
  <footer>
    <div class="container">
      <footerBuyMenu />
      <footerCenter />
      <footerBottom />
    </div>
  </footer>
</template>

<script>
import footerBuyMenu from './footerBuyMenu.vue'
import footerCenter from './footerCenter.vue'
import footerBottom from './footerBottom.vue'

export default {
  name: 'Footer',
  components:{
  footerBuyMenu,
  footerCenter,
  footerBottom,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>

</style>
