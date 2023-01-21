<script>
export default {
    name: 'AppFooter'

}
</script>

<template>
    <footer>
        <div class="container footer-content">
            <div class="sign-up">
                <button><a href="#">SIGN-UP NOW!</a></button>
            </div>
            <div class="links-footer">
                <div class="icon-claim">
                    <h2>FOLLOW US</h2>
                </div>
                <nav class="icon-footer">
                    <li><a href="#"><img src="../assets/img/footer-facebook.png" alt="facebook"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-twitter.png" alt="facebook"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-youtube.png" alt="facebook"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-pinterest.png" alt="facebook"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-periscope.png" alt="facebook"></a></li>
                </nav>
            </div>
        </div>
    </footer>

</template>

<style scoped>
/* Footer */
footer {
    background-color: #2c2c2c;
    height: 120px;
    position: relative;
}

/* Left footer */
.footer-content {
    display: flex;
    align-items: center;
    justify-content: space-between;
}

/* Right footer */
.links-footer {
    display: flex;
    align-items: center;
    justify-content: center;
}



.icon-footer {
    display: flex;
    align-items: center;
}

.icon-footer li {
    padding: 0 10px;
}

/* Utils */
.sign-up button {
    padding: 10px;
    background-color: #2c2c2c;
    border-radius: 3px;
    border: 3px solid #1a75ff;
    cursor: pointer;
}

.sign-up a {
    color: white;
}

.icon-claim {
    margin-right: 10px;
}

.icon-claim h2 {
    color: #1a75ff;
}
</style>