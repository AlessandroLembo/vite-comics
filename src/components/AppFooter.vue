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
                <p>FOOTER BOTTOM</p>
            </div>
        </div>
    </footer>

</template>

<style scoped>
.footer-top {
    background-color: brown;
    min-height: 350px;
}

.footer-bottom {
    background-color: cornflowerblue;
    min-height: 350px;
}
</style>