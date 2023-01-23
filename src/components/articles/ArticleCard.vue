<script>

export default {
    name: 'ArticleCard',
    props: {
        article: Object
    },


}
</script>

<template>
    <div class="card">
        <img :src="article.thumb" :alt="article.type">
        <h3> {{ article.series }} </h3>
    </div>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/mixins' as *;
@use '../../assets/scss/partials/variables' as *;

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