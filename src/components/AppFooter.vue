<script>
export default {
    name: 'AppFooter'

}
</script>

<template>
    <footer>
        <div class="footer-top">
            <div class="container">
                <p>FOOTER TOP</p>
            </div>
        </div>
        <div class="footer-bottom">
            <div class="container">
                <div class="link-lists">
                    <div class="left-lists">
                        <nav class="top-list">
                            <h2 class="title-list">DC COMICS</h2>
                            <ul>
                                <li><a href="#">acqua</a></li>

                            </ul>
                        </nav>
                        <nav class="bottom-list">
                            <h2 class="title-list">SHOP</h2>
                            <ul>
                                <li><a href="#">acqua</a></li>
                            </ul>
                        </nav>
                    </div>
                    <nav class="center-list">
                        <h2 class="title-list">DC</h2>
                        <ul>
                            <li><a href="#">acqua</a></li>
                        </ul>
                    </nav>
                    <nav class="right-list">
                        <h2 class="title-list">SITES</h2>
                        <ul>
                            <li><a href="#">acqua</a></li>
                        </ul>
                    </nav>
                </div>
                <figure>
                    <img src="" alt="">
                </figure>
            </div>
        </div>
    </footer>

</template>

<style scoped>
.footer-top {
    background-image: url('../assets/img/footer-bg.jpg');
    background-position: cover;
    background-size: cover;
    background-repeat: no-repeat;
    min-height: 350px;
}

.link-lists {
    display: flex;
    align-items: center;
}

.footer-bottom {
    background-color: cornflowerblue;
    min-height: 350px;
}
</style>