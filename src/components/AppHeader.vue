<script>
export default {
    data() {
        return {

        }
    }
}
</script>


<template>
    <header>
        <div class="container-centered">

            <div class="header-item">
                <img src="/img/buy-comics-digital-comics.png" alt="">
                <div class="header-item-text">DIGITAL COMICS</div>
            </div>
            <div class="header-item">
                <img src="/img/buy-comics-merchandise.png" alt="">
                <div class="header-item-text">DC MERCHANDISE</div>
            </div>
            <div class="header-item">
                <img src="/img/buy-comics-subscriptions.png" alt="">
                <div class="header-item-text">SUBSCRIPTION</div>
            </div>
            <div class="header-item">
                <img src="/img/buy-comics-shop-locator.png" alt="">
                <div class="header-item-text">COMIC SHOP LOCATOR</div>
            </div>
            <div class="header-item">
                <img src="/img/buy-dc-power-visa.svg" alt="">
                <div class="header-item-text">DC POWER VISA</div>
            </div>
        </div>
    </header>
</template>



<style lang="scss" scoped>
header {
    height: 140px;
    background-color: rgb(2, 119, 248);

    .container-centered {
        display: flex;
        justify-content: space-around;
        padding: 0 30px;
        gap: 40px;
        height: 100%;

        .header-item {
            display: flex;
            align-items: center;
            gap: 8px;
            font-size: 0.7em;
            color: white;
            font-weight: bold;

            & img {
                width: 40px;
            }

            &:nth-child(4) img {
                width: 32px;
            }
        }
    }


}
</style>