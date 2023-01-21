<script>
export default {
    name: 'AppMainContent'

}
</script>

<template>
    <section id="links-main">
        <nav class="container ">
            <ul class="main-images">
                <li class="choose-operations">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="digital comics">
                    <h4>DIGITAL COMICS</h4>
                </li>
                <li class="choose-operations">
                    <img src="../assets/img/buy-comics-merchandise.png" alt="merchandise">
                    <h4>DIGITAL COMICS</h4>
                </li>
                <li class="choose-operations">
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="subscription">
                    <h4>DIGITAL COMICS</h4>
                </li>
                <li class="choose-operations">
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="comic schop">
                    <h4>DIGITAL COMICS</h4>
                </li>
                <li class="choose-operations">
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="power visa">
                    <h4>DIGITAL COMICS</h4>
                </li>
            </ul>
        </nav>
    </section>

</template>

<style scoped>
/* SECTION MAIN LINKS */
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
}
</style>