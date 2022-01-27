<template>
  <header>
    <div class="container">
        logo
        <headerNav />
    </div>
  </header>
</template>

<script>
import headerNav from './headerNav.vue'

export default {
  name: 'Header',
  components: {
    headerNav,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import '../assets/style/partials/variables.scss';
header{
  text-align: center;
}
nav{
  display: flex;
  justify-content: center;

    ul{
      list-style: none;
      display: flex;
    }
    
    li a{
      display: inline-block;
      color: black;
      padding: 15px 20px;
      text-decoration: none;

        &.active,&:hover{
          background-color: $secondary_color;
        }
    }
}
.container{
    max-width: 600px; /* non vado a modificare il .container nel global
    perchè ci sta scoped ///// da togliere sto container*/
}
</style>
