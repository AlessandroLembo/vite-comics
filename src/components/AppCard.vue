<script>
export default {

}
</script>

<template>
    <section id="content-top">
        <div class="container main-top-content">
            <h2>-- Content goes here --</h2>
            <p>Cards</p>
        </div>
    </section>

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
</style>