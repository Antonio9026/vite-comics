<script >

export default {
    name: "AppBanner",

}

</script>

<template>
    <div class="banner_container">
        <div class="card">
            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
            <p>DIGITAL COMICS</p>
        </div>
        <div class="card">
            <img src="../assets/img/buy-comics-merchandise.png" alt="">
            <p>DIGITAL MERCHANDISE</p>
        </div>
        <div class="card">
            <img src="../assets/img/buy-comics-shop-locator.png" alt="">
            <p>SUBSCRIPTION</p>
        </div>
        <div class="card">
            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
            <p>COMIC SHOP LOCATOR</p>
        </div>
        <div class="card">
            <img src="../assets/img/buy-dc-power-visa.svg" alt="">
            <p>DC POWER VISA</p>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.banner_container {
    height: 150px;
    display: flex;
    justify-content: center;
    gap: 20px;
    background-color: #0282f9;

    .card {
        display: flex;
        align-items: center;
        font-size: 11px;
        gap: 10px;

        img {
            height: 50px;
        }
    }
}




</style>
