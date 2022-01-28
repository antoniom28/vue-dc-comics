<template>
    <div class="button-div">
        <a href="#">
            {{textButton}}
        </a>
    </div>
</template>

<script>
export default {
    name: "mainButton",
    props: {
        textButton : String,
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/partials/variables.scss';

.button-div a{
    color: white;
    background-color: $main_color;
    font-weight: bold;
}
</style>