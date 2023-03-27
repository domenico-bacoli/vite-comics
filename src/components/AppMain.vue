<script>
import AppBluBandSection from './AppBluBandSection.vue';
import AppComicBookSeries from './AppComicBookSeries.vue';


export default {
    data() {
        return {

            comicBookSeries: [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ],
        };
    },

    components: {
        AppBluBandSection,
        AppComicBookSeries,
    }
}
</script>


<template>
    <div class="main">
        <div class="main-image">

        </div>
        <div class="container-centered">
            <div class="main-title-absolute">CURRENT SERIES</div>
            <div class="card-series-container">
                <AppComicBookSeries v-for="comicBook in comicBookSeries" :img="comicBook.thumb" :title="comicBook.series">
                </AppComicBookSeries>
            </div>
            <div class="button-load">
                <button>LOAD MORE</button>
            </div>
        </div>
    </div>
    <AppBluBandSection></AppBluBandSection>
</template>



<style lang="scss" scoped>
.main {
    display: flex;
    flex-direction: column;
    display: flex;
    align-items: center;
    width: 100%;

    .main-image {
        position: relative;
        height: 280px;
        width: 100%;
        background-image: url(/img/jumbotron.jpg);
        background-size: cover;
    }

    .container-centered {
        position: relative;

        .main-title-absolute {
            position: absolute;
            top: -24px;
            left: -14px;
            color: white;
            background-color: rgb(2, 119, 248);
            padding: 8px 22px;
            font-size: 1.2em;
            font-weight: bold;
        }
    }

    .card-series-container {
        display: flex;
        flex-flow: row wrap;
        justify-content: center;
        gap: 20px;
        padding: 50px 0 40px;
    }

    .button-load {
        text-align: center;
        padding-bottom: 16px;

        button {
            background-color: rgb(2, 119, 248);
            color: white;
            font-weight: bold;
            padding: 10px 30px;
            border-radius: 2px;
            border: none;
            cursor: pointer;
        }
    }
}
</style>