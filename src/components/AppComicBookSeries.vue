<script>

export default {
    data() {
        return {

        };
    },

    props: {
        img: String,
        title: String,
    },
}
</script>


<template>
    <div class="card-container container-centered">
        <div class="card-series">
            <img :src="img" alt="series image">

        </div>
        <div class="series-title">{{ title }}</div>
    </div>
</template>


<style lang="scss" scoped>
.card-container {
    width: calc(100% / 6 - (20px / 6 * 5));

    .card-series {
        height: 150px;
        overflow: hidden;

        img {
            width: 100%;
        }
    }

    .series-title {
        color: white;
        text-transform: uppercase;
        font-size: 0.62em;
        font-weight: bold;
        padding-top: 8px;
    }
}
</style>