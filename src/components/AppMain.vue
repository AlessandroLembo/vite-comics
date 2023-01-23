<script>
import AppMainContent from './AppMainContent.vue';
export default {
    name: 'AppMain',
    components: { AppMainContent }

}
</script>

<template>
    <main>
        <section id="content-top">
            <div class="container main-top-content">
                <h2>-- Content goes here --</h2>
                <p>Cards</p>
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

/* SECTION TOP CONTENT */
#content-top {
    background-color: rgba(0, 0, 0, 0.8);
    min-height: 130px;
}

.main-top-content {
    min-height: $h100;
    @include vertical_algnm;
}

h2,
p {
    height: $h100;
    @include vertical_algnm;
    margin: 1rem auto;
    color: white;
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