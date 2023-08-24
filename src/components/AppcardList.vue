<script>
export default {
    props: {
        thumb: String,
        series: String,
    }

}
</script>



<template>
    <div class="card">
        <div class="img-container">
            <img :src="thumb" alt="">
        </div>
        <div class="series">
            <strong> {{ series.toUpperCase() }}</strong>
        </div>
    </div>
</template>


<style lang="scss" scoped>
.card {
    width: calc(100% / 6);
    margin: 10px 0;
    .img-container {
        width: 140px;
        height: 140px;
        margin: 10px 0;

        img {
            width: 100%;
        }
    }

    .series {
        max-width: 140px;
        color: white;
        font-size: 11px;
    }
}
</style>