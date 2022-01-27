<template>
  <header>
    <div class="container">
      <div class="logo">
      </div>
      <nav>
        <ul>
          <li :key="index" v-for="(item,index) in menuItem">
            <a :href="item.href" >{{item.text}}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'headerNav',
  data(){
    return{
      menuItem : [
        {
          text : "CHARACTERS",
          href : "#",
        },
        {
          text : "COMICS",
          href : "#",
        },
        {
          text : "MOVIES",
          href : "#",
        },
        {
          text : "TV",
          href : "#",
        },
        {
          text : "GAMES",
          href : "#",
        },
        {
          text : "COLLECTIBLES",
          href : "#",
        },
        {
          text : "VIDEOS",
          href : "#",
        },
        {
          text : "FANS",
          href : "#",
        },
        {
          text : "NEWS",
          href : "#",
        },
        {
          text : "SHOP",
          href : "#",
        },
      ],
    }
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
