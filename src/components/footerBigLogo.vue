<template>
    <div class="container">
        <div class="logo"></div>
    </div>
</template>

<script>
export default{
    name:"footerBigLogo",
}
</script>

<style lang="scss" scoped>
.container{

    .logo{
        min-width: 580px;
        height: 100%;
        background-image: url('../assets/img/dc-logo-bg.png');
        background-size: auto;
        background-position: center center;
        background-repeat: no-repeat;
    }
}
</style>