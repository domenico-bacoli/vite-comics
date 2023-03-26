<script>
export default {
    data() {
        return {

            mainList: [
                {
                    title: 'DC COMICS',
                    mainLinks: [
                        'Characters',
                        'Comics',
                        'Movies',
                        'Tv',
                        'Games',
                        'Videos',
                        'News',
                    ],
                },
                {
                    title: 'DC',
                    mainLinks: [
                        'Terms Of Use',
                        'Privacy policy (New)',
                        'Ad Choices',
                        'Advertising',
                        'Jobs',
                        'Subscriptions',
                        'Talent Workshops',
                        'CPSC Certificates',
                        'Ratings',
                        'Shop Help',
                        'Contact Us',
                    ],
                },
                {
                    title: 'SITES',
                    mainLinks: [
                        'DC',
                        'MAD Magazine',
                        'DC Kids',
                        'DC Universe',
                        'DC Power Visa',
                    ],
                },
                {
                    title: 'SHOP',
                    mainLinks: [
                        'Shop DC',
                        'Shop DC Collectibles',
                    ],
                },
            ],
        }
    },
}
</script>


<template>
    <footer>
        <div class="container-centered">
            <div class="footer-list">
                <div v-for="item in mainList" class="col">
                    <strong class="list-title">{{ item.title }}</strong>
                    <ul>
                        <li v-for="link in item.mainLinks" class="list-element">{{ link }}</li>
                    </ul>
                </div>

            </div>
        </div>
    </footer>
</template>


<style lang="scss" scoped>
footer {
    background-image: url(/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;

    .container-centered {
        background-image: url(/img/dc-logo-bg.png);
        background-repeat: no-repeat;
        background-position: right;
        background-size: 50%;
    }

    .footer-list {
        display: flex;
        flex-flow: row wrap;
        gap: 40px;
        width: 50%;
        padding-top: 30px;

        li {
            color: rgb(155, 155, 155);
            font-size: 0.7em;
        }

        .col {
            height: 120px;

            strong {
                color: white;
            }

            .list-title {
                margin-bottom: 20px;
            }
        }
    }
}
</style>