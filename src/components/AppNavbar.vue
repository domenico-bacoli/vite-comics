<script>

export default {
    data() {
        return {
            navLinks: [
                'CHARACTERS',
                'COMICS',
                'MOVIES',
                'TV',
                'GAMES',
                'COLLECTIBLES',
                'VIDEOS',
                'FANS',
                'NEWS',
                'SHOP'
            ],

            activeIndex: 0,
        }
    },

    methods: {
        activeLink(index) {
            this.activeIndex = index;
        }
    }
}

</script>


<template>
    <nav>
        <div class="container-centered">
            <div class="logo">
                <img src="/img/dc-logo.png" alt="logo DC">
            </div>
            <ul>
                <li v-for="(link, index) in navLinks" @click="activeLink(index)"
                    :class="activeIndex == index ? 'active' : ''">{{
                        link }}</li>
            </ul>
        </div>
    </nav>
</template>



<style lang="scss" scoped>
nav {
    height: 100px;
    background-color: white;

    .container-centered {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100%;

        .logo {
            display: flex;
            align-items: center;

            img {
                width: 70px;
            }
        }
    }

    ul {
        display: flex;
        align-items: center;
        gap: 22px;
        font-size: .7em;
        font-weight: bold;
        height: 100%;
    }

    li {
        height: 100%;
        display: flex;
        align-items: center;
        cursor: pointer;

        &.active {
            color: rgb(2, 119, 248);
            border-top: 5px solid transparent;
            border-bottom: 5px solid rgb(2, 119, 248);
        }
    }
}
</style>