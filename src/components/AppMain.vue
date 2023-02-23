<script>
import AppMainContent from './AppMainContent.vue';
import ArticleCard from './articles/ArticleCard.vue';
import BannerImage from './BannerImage.vue';


export default {
    name: 'AppMain',
    components: { AppMainContent, ArticleCard, BannerImage },
    data() {
        return {
            articles: [
                {
                    thumb: 'https://static.dc.com/2023-02/SHZAM2_INSTA_MAIN_900x900_DOM.jpg?w=900',
                    price: '$19.99',
                    series: 'Action Comics',
                    type: 'comic book',
                },
                {
                    thumb: 'https://static.dc.com/dc/files/default_images/DCConnect_33-1_63cadf27012cc7.90969922.jpg?w=640',
                    price: '$3.99',
                    series: 'American Vampire 1976',
                    type: 'comic book',
                },
                {
                    thumb: 'https://static.dc.com/dc/files/default_images/WWV3%2520TVOOF%2528%2520Cover%2529_63d2c26e350cb7.59228985.jpg?w=640',
                    price: '$16.99',
                    series: 'Aquaman',
                    type: 'graphic novel',
                },
                {
                    thumb: 'https://static.dc.com/dc/files/default_images/TSWTH_v3%2520%2528Cover%2529_63d02da77073c9.49320677.jpg?w=640',
                    price: '$2.99',
                    series: 'Batgirl',
                    type: 'comic book',
                },
                {
                    thumb: 'https://static.dc.com/dc/files/default_images/SANDMAN%2520Bk5%2520%2528Cover%2529_63d2c25d6283c5.65185483.jpg?w=640',
                    price: '$3.99',
                    series: 'Batman',
                    type: 'comic book',
                },
                {
                    thumb: 'https://static.dc.com/dc/files/default_images/THEJKR_v3%2520%2528Cover%2529_63dbf9ea07e299.23790036.jpg?w=640',
                    price: '$2.99',
                    series: 'Batman Beyond',
                    type: 'comic book',
                },
                {
                    thumb: 'https://static.dc.com/dc/files/default_images/THEJKR_v3%2520%2528Cover%2529_63dbf9ea07e299.23790036.jpg?w=640',
                    price: '$3.99',
                    series: 'Batman/Superman',
                    type: 'comic book',
                },
                {
                    thumb: 'https://static.dc.com/dc/files/default_images/SANDMAN%2520Bk5%2520%2528Cover%2529_63d2c25d6283c5.65185483.jpg?w=640',
                    price: '$4.99',
                    series: 'Batman/Superman Annual',
                    type: 'comic book',
                },
                {
                    thumb: 'https://static.dc.com/dc/files/default_images/TSWTH_v3%2520%2528Cover%2529_63d02da77073c9.49320677.jpg?w=640',
                    price: '$5.99',
                    series: 'Batman: The Joker War Zone',
                    type: 'comic book',
                },
                {
                    thumb: 'https://static.dc.com/dc/files/default_images/WWV3%2520TVOOF%2528%2520Cover%2529_63d2c26e350cb7.59228985.jpg?w=640',
                    price: '$6.99',
                    series: 'Batman: Three Jokers',
                    type: 'comic book',
                },
                {
                    thumb: 'https://static.dc.com/dc/files/default_images/DCConnect_33-1_63cadf27012cc7.90969922.jpg?w=640',
                    price: '$4.99',
                    series: 'Batman: White Knight Presents: Harley Quinn',
                    type: 'comic book',
                },
                {
                    thumb: 'https://static.dc.com/2023-02/SHZAM2_INSTA_MAIN_900x900_DOM.jpg?w=900',
                    price: '$16.99',
                    series: 'Catwoman',
                    type: 'graphic novel',
                }
            ]
        }
    },

}
</script>

<template>
    <main>
        <banner-image></banner-image>

        <section id="content-top">
            <div class="container cards-section">
                <button id="current-series">CURRENT SERIES</button>
                <div class="main-top-content">
                    <div class="main-top-content">
                        <div v-for="article in articles" :key="article.series" class="col">
                            <article-card :article="article"></article-card>
                        </div>
                    </div>
                    <button id="load">LOAD MORE</button>
                </div>
            </div>
        </section>

        <app-main-content></app-main-content>


        <section id="jumbotron">
            <div class="container jumbo-container">
                <div class="link-lists">
                    <div class="left-lists">
                        <nav class="top-list">
                            <h2 class="title-list">DC COMICS</h2>
                            <ul>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Comics</a></li>
                                <li><a href="#">Movies</a></li>
                                <li><a href="#">TV</a></li>
                                <li><a href="#">Games</a></li>
                                <li><a href="#">Videos</a></li>
                                <li><a href="#">News</a></li>
                            </ul>
                        </nav>
                        <nav class="bottom-list">
                            <h2 class="title-list">SHOP</h2>
                            <ul>
                                <li><a href="#">Shop DC</a></li>
                                <li><a href="#">Shop DC Collectibles</a></li>
                            </ul>
                        </nav>
                    </div>
                    <nav class="center-list">
                        <h2 class="title-list">DC</h2>
                        <ul>
                            <li><a href="#">Terms Of Use</a></li>
                            <li><a href="#">Privacy policy (New)</a></li>
                            <li><a href="#">Ad Choices</a></li>
                            <li><a href="#">Advertising</a></li>
                            <li><a href="#">Jobs</a></li>
                            <li><a href="#">Subscriptions</a></li>
                            <li><a href="#">Talent Workshops</a></li>
                            <li><a href="#">CPSC Certificates</a></li>
                            <li><a href="#">Ratings</a></li>
                            <li><a href="#">Shop Help</a></li>
                            <li><a href="#">Contact Us</a></li>
                        </ul>
                    </nav>
                    <nav class="right-list">
                        <h2 class="title-list">SITES</h2>
                        <ul>
                            <li><a href="#">DC</a></li>
                            <li><a href="#">MAD Magazine</a></li>
                            <li><a href="#">DC Kids</a></li>
                            <li><a href="#">DC Universe</a></li>
                            <li><a href="#">DC Power Visa</a></li>
                        </ul>
                    </nav>
                </div>
                <figure>
                    <img src="../assets/img/dc-logo-bg.png" alt="logo">
                </figure>
            </div>
        </section>

    </main>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/mixins' as *;
@use '../assets/scss/partials/variables' as *;
@use '../assets/scss/partials/buttons.scss' as *;


/* SECTION TOP CONTENT */
#content-top {
    background-color: rgba(0, 0, 0, 0.8);
    min-height: 130px;

    .cards-section {
        position: relative;

        #current-series {
            @include btn-style;
            width: 280px;
            height: 50px;
            padding: 15px 20px;
            font-size: 18px;
            position: absolute;
            left: 0;
            top: -25px;
        }

        .main-top-content {
            min-height: $h100;
            @include vertical_algnm;
            flex-wrap: wrap;
            padding: 1rem 0;

            .col {
                flex-basis: calc(100% / 6);
                height: 240px;
                margin: 2rem auto 0.5rem;
                padding: 0 1rem;
            }
        }

        #load {
            @include btn-style;
            width: 180px;
            padding: 10px 5px;
            margin: 1rem auto;
        }
    }

}



/* SECTION JUMBOTRON */
#jumbotron {
    background-image: url('../assets/img/footer-bg.jpg');
    background-position: cover;
    background-size: cover;
    background-repeat: no-repeat;
    height: 450px;

}

.jumbo-container {
    @include vertical_algnm;
    justify-content: space-between;
    height: $h100;
}

.link-lists {
    display: flex;
    align-items: flex-start;
    height: 100%;
    margin-top: 8rem;

    li {
        padding-bottom: 3px;
    }

    a {
        color: rgba(255, 255, 255, 0.3);
    }
}

.jumbo-container figure {
    height: $h100;
    @include vertical_algnm;
}

.jumbo-container img {
    height: 140%;
}


/* Utils */
.top-list {
    margin-bottom: 1.5rem;
}

.center-list {
    margin: 0 2rem;
}

h2 {
    margin-bottom: 1rem;
}
</style>