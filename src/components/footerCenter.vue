<template>
  <footer>
    <div class="container-bg">
      <div class="footer-container">
        <footerSubLinks />
        <footerBigLogo />
      </div>
    </div>
  </footer>
</template>

<script>
import footerSubLinks from './footerSubLinks.vue'
import footerBigLogo from './footerBigLogo.vue'

export default {
  name: 'footerCenter',
  components: {
    footerSubLinks,
    footerBigLogo,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>

.container-bg{
  background-image: url(../assets/img/footer-bg.jpg);
}

.footer-container{
  display: flex;
  justify-content: space-around;
}
</style>
