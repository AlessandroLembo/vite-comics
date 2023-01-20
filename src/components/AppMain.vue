<script>
export default {
    name: 'AppMain',

}
</script>

<template>
    <main>
        <div class="content-top">
            <div class="container main-top-content">
                <h2>--CONTENT--</h2>
            </div>
        </div>
        <div class="content-bottom">
            <div class="container">
                <h2>ICON</h2>
            </div>
        </div>

    </main>

</template>

<style scoped>
/* TOP CONTENT */
main {
    height: calc(100vh - 620px);
    overflow-y: auto;
}

.content-top {
    background-color: rgba(0, 0, 0, 0.8);
    height: 120px;
}

.container.main-top-content {
    height: 100%;
}

h2 {
    height: 100%;
    display: flex;
    align-items: center;
}

/* BOTTOM CONTENT */
.content-bottom {
    background-color: dodgerblue;
    min-height: calc((100vh - 620px) - 120px);
    position: relative;
}

/* Utils */
h2 {
    color: white;
}
</style>