<script>
export default {
    name: 'AppMain',

}
</script>

<template>
    <main>
        <section id="content-top">
            <div class="container main-top-content">
                <h2>--CONTENT--</h2>
            </div>
        </section>
        <section id="links-main">
            <div class="container main-images">

            </div>
        </section>
        <section id="jumbotron">
            <div class="container jumbo-container">
                <div class="link-lists">
                    <div class="left-lists">
                        <nav class="top-list">
                            <h2 class="title-list">DC COMICS</h2>
                            <ul>
                                <li><a href="#">Movies</a></li>
                                <li><a href="#">Movies</a></li>
                                <li><a href="#">Movies</a></li>
                                <li><a href="#">Movies</a></li>
                                <li><a href="#">Movies</a></li>
                                <li><a href="#">Movies</a></li>
                                <li><a href="#">Movies</a></li>
                            </ul>
                        </nav>
                        <nav class="bottom-list">
                            <h2 class="title-list">SHOP</h2>
                            <ul>
                                <li><a href="#">Movies</a></li>
                                <li><a href="#">Movies</a></li>
                            </ul>
                        </nav>
                    </div>
                    <nav class="center-list">
                        <h2 class="title-list">DC</h2>
                        <ul>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">Movies</a></li>
                        </ul>
                    </nav>
                    <nav class="right-list">
                        <h2 class="title-list">SITES</h2>
                        <ul>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">Movies</a></li>
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

/* SECTION MAIN LINKS */
#links-main {
    background-color: dodgerblue;
    height: 150px;
    position: relative;
}

.main-images {
    display: flex;
}

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