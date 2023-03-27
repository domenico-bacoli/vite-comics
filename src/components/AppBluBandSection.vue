<script>
export default {
    data() {
        return {
            headerItems: [
                {
                    title: 'DIGITAL COMICS',
                    image: '/img/buy-comics-digital-comics.png',
                },
                {
                    title: 'DC MERCHANDISE',
                    image: '/img/buy-comics-merchandise.png',
                },
                {
                    title: 'SUBSCRIPTION',
                    image: '/img/buy-comics-subscriptions.png',
                },
                {
                    title: 'COMIC SHOP LOCATOR',
                    image: '/img/buy-comics-shop-locator.png',
                },
                {
                    title: 'DC POWER VISA',
                    image: '/img/buy-dc-power-visa.svg',
                },
            ],
        }
    },
}
</script>


<template>
    <section class="blu-band">
        <div class="container-centered">
            <div v-for="item in headerItems" class="section-item">
                <img :src="item.image" :alt="item.title">
                <div class="section-item-text">{{ item.title }}</div>
            </div>
        </div>

    </section>
</template>


<style lang="scss" scoped>
section {
    height: 120px;
    background-color: rgb(2, 119, 248);

    .container-centered {
        display: flex;
        justify-content: space-around;
        padding: 0 30px;
        gap: 40px;
        height: 100%;

        .section-item {
            display: flex;
            align-items: center;
            gap: 8px;
            font-size: 0.7em;
            color: white;
            font-weight: bold;

            & img {
                width: 38px;
            }

            &:nth-child(4) img {
                width: 28px;
            }
        }
    }
}
</style>