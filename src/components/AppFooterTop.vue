<script>
export default {
    data() {
        return {

            footerLinks: [
                {
                    title: 'DC COMICS',
                    links: [
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
                    title: 'SHOP',
                    links: [
                        'Shop DC',
                        'Shop DC Collectibles',
                    ],
                },
                {
                    title: 'DC',
                    links: [
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
                    links: [
                        'DC',
                        'MAD Magazine',
                        'DC Kids',
                        'DC Universe',
                        'DC Power Visa',
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
                <div v-for="item in footerLinks" class="col">
                    <strong class="list-title">{{ item.title }}</strong>
                    <ul>
                        <li v-for="link in item.links" class="list-element">{{ link }}</li>
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
        flex-flow: column wrap;
        justify-content: flex-start;
        align-items: flex-start;
        align-content: flex-start;
        gap: 30px;
        padding-top: 30px;
        height: 320px;

        li {
            color: rgb(155, 155, 155);
            font-size: 0.7em;
        }

        .col {

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