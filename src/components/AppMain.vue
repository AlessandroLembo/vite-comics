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

<style scoped>
/* SECTION TOP CONTENT */
#content-top {
    background-color: rgba(0, 0, 0, 0.8);
    height: 120px;
}

.main-top-content {
    height: 100%;
}

h2 {
    height: 100%;
    display: flex;
    align-items: center;
}

/* SECTION MAIN LINKS
#links-main {
    background-color: dodgerblue;
    height: 150px;
    position: relative;
}

.main-images {
    display: flex;
    justify-content: space-around;
    align-items: center;
    height: 100%;
}

.choose-operations {
    display: flex;
    align-items: center;
    height: 100%;
}

.choose-operations img {
    height: 70px;
    margin-right: 10px;
}

.main-images li:last-child img {
    height: 45px;
} */

/* SECTION JUMBOTRON */
#jumbotron {
    background-image: url('../assets/img/footer-bg.jpg');
    background-position: cover;
    background-size: cover;
    background-repeat: no-repeat;
    height: calc(100vh - 510px);

}

.jumbo-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}


.link-lists {
    display: flex;
    align-items: flex-start;
}

.link-lists li {
    padding-bottom: 3px;
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

.link-lists a {
    color: rgba(255, 255, 255, 0.3);
}
</style>