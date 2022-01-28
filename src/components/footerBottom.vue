<template>
    <div class="container">
      <footerButton />
      <footerSocial />
    </div>
</template>

<script>
import footerButton from './footerButton.vue'
import footerSocial from './footerSocial.vue'

export default {
  name: 'footerBottom',
  components: {
    footerButton,
    footerSocial,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import '../assets/style/partials/variables.scss';
.container{
  padding: 10px 0;
  background-color: $third-color;
  display: flex;
  justify-content: space-around;
  align-items: center;
}

</style>
