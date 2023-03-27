<script>
export default {
    data() {
        return {

            footerSocialIcon: [
                '/img/footer-facebook.png',
                '/img/footer-twitter.png',
                '/img/footer-youtube.png',
                '/img/footer-pinterest.png',
                '/img/footer-periscope.png',
            ],
        }
    },
}
</script>


<template>
    <footer>
        <div class="container-centered">
            <div class="footer-button">
                <button>SIGN-UP NOW!</button>
            </div>
            <div class="footer-social-link">
                <span>FOLLOW US</span>
                <img v-for="icon in footerSocialIcon" :src="icon" alt="social icon">
            </div>
        </div>

    </footer>
</template>



<style lang="scss" scoped>
footer {
    background-color: rgb(48, 48, 48);
    height: 100px;

    .container-centered {
        width: 100%;
        height: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .footer-button {
        button {
            padding: 10px 16px;
            border: 2px solid rgb(2, 119, 248);
            background-color: rgb(48, 48, 48);
            color: white;
            font-weight: bold;
            cursor: pointer;
        }
    }

    .footer-social-link {
        display: flex;
        align-items: center;
        gap: 14px;

        span {
            color: rgb(2, 119, 248);
            font-weight: bold;
        }

        img {
            cursor: pointer;
        }
    }
}
</style>