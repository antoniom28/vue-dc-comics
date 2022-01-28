<template>
    <div class="container standard-button">
        <a href="#">SIGN-UP NOW!</a>
    </div>
</template>

<script>
export default {
    name: "footerButton",
}
</script>

<style lang="scss" scoped>
@import '../assets/style/partials/variables.scss';

a{
    color:white;
    padding: 10px 10px;
    border: 2px solid $main_color;
    /*box-shadow: 0px 0px 0px 2px $main_color;*/
}
</style>