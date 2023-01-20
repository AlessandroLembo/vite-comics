<script>
export default {
    name: 'AppFooter'

}
</script>

<template>
    <footer>
        <div class="footer-top">
            <div class="container footer-content">
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
        </div>
        <div class="footer-bottom">
            <div class="container">

            </div>
        </div>
    </footer>

</template>

<style scoped>
footer {
    height: 500px;
}

.footer-top {
    background-image: url('../assets/img/footer-bg.jpg');
    background-position: cover;
    background-size: cover;
    background-repeat: no-repeat;
    height: 380px;
}

.footer-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.link-lists {
    display: flex;
    /* padding: 2rem 0; */
}

.top-list {
    margin-bottom: 1.5rem;
}

.center-list {
    margin: 0 2rem;
}

.footer-bottom {
    background-color: cornflowerblue;
    min-height: 120px;
    position: relative;
}

/* Utils */
h2 {
    color: white;
    margin-bottom: 1rem;
}

.link-lists a {
    color: rgba(255, 255, 255, 0.3);
}
</style>