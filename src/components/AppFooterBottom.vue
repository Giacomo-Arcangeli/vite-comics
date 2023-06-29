<script>
export default {
    data() {
        return {}
    }
}
</script>

<template>
    <footer class="footer-bottom">
        <div class="container">
            <a href="#">SIGN-UP NOW!</a>
            <ul>
                <li>
                    <h3>FOLLOW US</h3>
                </li>
                <li><img src="../assets/img/footer-facebook.png" alt=""></li>
                <li><img src="../assets/img/footer-twitter.png" alt=""></li>
                <li><img src="../assets/img/footer-youtube.png" alt=""></li>
                <li><img src="../assets/img/footer-pinterest.png" alt=""></li>
                <li><img src="../assets/img/footer-periscope.png" alt=""></li>
            </ul>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
footer {
    background-color: rgb(48, 48, 48);
    height: 120px;
}

.container {
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

ul {
    display: flex;
    align-items: center;
}

li {
    margin: 0 10px;
}

h3 {
    color: rgb(2, 130, 249);
}

a {
    color: white;
    padding: 10px 15px;
    border: 2px solid rgb(2, 130, 249);
}

img {
    cursor: pointer;
}
</style>