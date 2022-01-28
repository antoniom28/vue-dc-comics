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
nav{
  font-size: 0.8em;
    ul{
      list-style: none;
      display: flex;
    }
    
    li a{
      display: inline-block;
      margin: 0px 20px;
      padding: 47px 0;

        &.active,&:hover{
          box-shadow: 0px 5px $main_color;
          color: $main_color;
        }
    }
}
</style>
