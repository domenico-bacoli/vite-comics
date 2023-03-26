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
                <li v-for="link in navLinks">{{ link }}</li>

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
    }
}
</style>