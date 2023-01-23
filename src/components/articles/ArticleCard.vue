<script>

export default {
    name: 'ArticleCard',
    props: {
        articles: Array
    },

}
</script>

<template>
    <section id="content-top">
        <div class="container main-top-content">
            <div v-for="article in articles" :key="article.series" class="col">
                <div class="card">
                    <img :src="article.thumb" :alt="article.type">
                    <h3> {{ article.series }} </h3>
                </div>
            </div>
        </div>
    </section>

</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/mixins' as *;
@use '../../assets/scss/partials/variables' as *;

/* SECTION TOP CONTENT */
#content-top {
    background-color: rgba(0, 0, 0, 0.8);
    min-height: 130px;
}

.main-top-content {
    min-height: $h100;
    @include vertical_algnm;
    flex-wrap: wrap;
    padding-bottom: 1.5rem;
}

.col {
    flex-basis: calc(100% / 6);
    height: 240px;
    margin: 2rem auto 0.5rem;
    padding: 0 1rem;
}

.card {
    height: $h100;

    img {
        height: 80%;
        width: 100%;
        object-fit: cover;
        object-position: 100% 0%;
        display: block;
    }

    h3 {
        padding-top: 10px;
        color: white;
        font-size: 15px;
    }
}
</style>