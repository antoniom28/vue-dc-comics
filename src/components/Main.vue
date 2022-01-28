<template>
  <main>
    <div class="container">
      <div class="jumbo"></div>
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
  },
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

.jumbo{
  width: 100%;
  height: 300px;
  background-image: url('../assets/img/jumbotron.jpg');
  background-size: cover;
}

</style>
