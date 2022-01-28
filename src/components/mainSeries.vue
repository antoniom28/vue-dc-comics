<template>
    <li class="serie">
        <a href="#">
            <div class="thumb">
                <img :src="currentSeries.thumb" :alt="currentSeries.series">
            </div>
        </a>
        <h4>{{currentSeries.series}}</h4>
    </li>
</template>

<script>
export default {
    name : "mainSeries",
    props: {
        currentSeries : Object,
    }
}
</script>

<style lang="scss" scoped>
li{
    width: 200px;
    
    .thumb{
        width: 200px;
        height: 200px;
        overflow: hidden;
        margin: 15px 0;
    }
}
</style>