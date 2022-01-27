<template>
  <footer>
    <div class="container">
        <ul>
            <li v-for="(item,index) in buyItems" :key="index">
              <img v-bind:src="item.image" alt="">
              <span>{{item.text}}</span>
            </li>
        </ul>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'footerBuyMenu',
  data(){
    return{
      buyItems : [
        {
          image : require('@/assets/img/buy-comics-digital-comics.png'),
          text : 'DIGITAL COMICS',
        },
        {
          image : require('@/assets/img/buy-comics-merchandise.png'),
          text : 'DC MERCHANDISE',
        },
        {
          image : require('@/assets/img/buy-comics-subscriptions.png'),
          text : 'SUBSCRIPTION',
        },
        {
          image : require('@/assets/img/buy-comics-shop-locator.png'),
          text : 'COMIC SHOP LOCATOR',
        },
        {
          image : require('@/assets/img/buy-dc-power-visa.svg'),
          text : 'DC POWER VISA',
        },
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import '../assets/style/partials/variables.scss';
.container{
    background-color: $main_color;

     ul {
       display: flex;
      justify-content: space-evenly;
      padding: 20px 50px;
     }

     ul li{
      display: flex;
      align-items: center;
      list-style: none;
      color: white;
      font-size: 0.9em;

      span{
        margin-left: 15px;
      }
    }
}

img{
  width: 50px;
  max-height: 55px;
}
</style>
