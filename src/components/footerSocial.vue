<template>
    <div class="container">
        <h3>FOLLOW US</h3>
        <ul>
            <li v-for="(item,index) in socialItems" :key="index">
                <a :href=item.href>
                    <img :src="item.icon" alt="">
                </a>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: "footerSocial",
    data(){
        return{
            socialItems : [
                {
                    name : "facebook",
                    href : "#",
                    icon : require("@/assets/img/footer-facebook.png"),
                },
                {
                    name : "twitter",
                    href : "#",
                    icon : require("@/assets/img/footer-twitter.png"),
                },
                {
                    name : "youtube",
                    href : "#",
                    icon : require("@/assets/img/footer-youtube.png"),
                },
                {
                    name : "pinterest",
                    href : "#",
                    icon : require("@/assets/img/footer-pinterest.png"),
                },
                {
                    name : "periscope",
                    href : "#",
                    icon : require("@/assets/img/footer-periscope.png"),
                },
                
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/partials/variables.scss';

h3{
    color: $main_color;
    margin: 0 15px;
}

ul li{
    display: inline-block;
    margin: 0 15px;
}
</style>