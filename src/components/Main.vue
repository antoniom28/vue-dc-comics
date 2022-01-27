<template>
  <main>
    <div class="container">
      <mainContent />
    </div>
  </main>
</template>

<script>
import mainContent from './mainContent.vue'

export default {
  name: 'Main',
  components: {
    mainContent,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import '../assets/style/partials/variables.scss';

.container{
  background-color: $sec_color;
  min-height: 100px; /* poi da togliere */
  color : white; /**/
}

</style>
