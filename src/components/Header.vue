<template>
  <header>
    <div class="container">
        <headerLogo />
        <headerNav />
    </div>
  </header>
</template>

<script>
import headerNav from './headerNav.vue'
import headerLogo from './headerLogo.vue'

export default {
  name: 'Header',
  components: {
    headerNav,
    headerLogo,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import '../assets/style/partials/variables.scss';

.container{
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 80%;
  margin: 0 auto;
}
</style>
