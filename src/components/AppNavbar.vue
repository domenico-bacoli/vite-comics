<script>

export default {
    data() {
        return {

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
                <li>CHARACTERS</li>
                <li>COMICS</li>
                <li>MOVIES</li>
                <li>TV</li>
                <li>GAMES</li>
                <li>COLLECTIBLES</li>
                <li>VIDEOS</li>
                <li>FANS</li>
                <li>NEWS</li>
                <li>SHOP</li>
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
        gap: 16px;
        font-size: .8em;
        font-weight: bold;
    }
}
</style>