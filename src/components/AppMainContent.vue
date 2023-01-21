<script>
export default {
    name: 'AppMainContent',
    data() {
        return {
            images: [
                {
                    picture: 'buy-comics-digital-comics.png',
                    alt: 'digital comics',
                    pictureTitle: 'DIGITAL COMICS',
                },
                {
                    picture: 'buy-comics-merchandise.png',
                    alt: 'merchandise',
                    pictureTitle: 'DC MERCHANDISE'
                },
                {
                    picture: 'buy-comics-subscriptions.png',
                    alt: 'subscription',
                    pictureTitle: 'SUBSCRIPTION'
                },
                {
                    picture: 'buy-comics-shop-locator.png',
                    alt: 'comic schop',
                    pictureTitle: 'COMIC SHOP LOCATOR'
                },
                {
                    picture: 'buy-dc-power-visa.svg',
                    alt: 'power visa',
                    pictureTitle: 'DC POWER VISA'
                },

            ]
        }
    },

    methods: {
        buildImagePath(image) {
            const url = new URL(`../assets/img/${image.picture}`, import.meta.url);
            return url.href;
        }
    }

}
</script>

<template>
    <section id="links-main">
        <nav class="container ">
            <ul class="main-images">
                <li v-for="image in images" class="choose-operations">
                    <img :src="buildImagePath(image)" :alt="image.alt">
                    <h4> {{ image.pictureTitle }} </h4>
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