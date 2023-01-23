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
                <li v-for="image in images" class="choose-operations" :key="image.pictureTitle">
                    <img :src="buildImagePath(image)" :alt="image.alt">
                    <h4> {{ image.pictureTitle }} </h4>
                </li>
            </ul>
        </nav>
    </section>

</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/mixins' as *;
@use '../assets/scss/partials/variables' as *;


/* SECTION MAIN LINKS */
#links-main {
    background-color: $dodger;
    height: 150px;
    position: relative;
}

.main-images {
    @include vertical_algnm;
    justify-content: space-around;
    height: $h100;

    li:last-child img {
        height: 45px;
    }
}

.choose-operations {
    @include vertical_algnm;
    height: $h100;

    img {
        height: 70px;
        margin-right: 10px;
    }
}
</style>