<script>
export default {
    data() {
        return {}
    }
}
</script>

<template>
    <main>
        <!-- top -->
        <section class="section-top">
            <div class="container">
                <h2>Content goes here</h2>
            </div>
        </section>

        <!-- bottom -->
        <section class="section-bottom">
            <ul class="container">
                <li>
                    <img class="small" src="../assets/img/buy-comics-digital-comics.png" alt="">
                    <a href="#">DIGITAL COMICS</a>
                </li>
                <li>
                    <img src="../assets/img/buy-comics-merchandise.png" alt="">
                    <a href="#">DC MERCHANDISE</a>
                </li>
                <li>
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                    <a href="#">SUBSCRIPTION</a>
                </li>
                <li>
                    <img class="small" src="../assets/img/buy-comics-shop-locator.png" alt="">
                    <a href="#">COMIC SHOP LOCATOR</a>
                </li>
                <li>
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                    <a href="#">DC POWER VISA</a>
                </li>
            </ul>
        </section>
    </main>
</template>

<style lang="scss" scoped>
.section-top {
    color: white;
    background-color: rgb(28, 28, 28);
    height: 140px;

    div {
        display: flex;
        align-items: center;
        height: 100%;
    }
}

.section-bottom {
    height: 160px;
    background-color: rgb(2, 130, 249);

    ul {
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: center;

        li {
            display: flex;
            align-items: center;
            margin: 0 40px;

            img {
                width: 50px;

            }

            a {
                color: white;
                padding: 0 10px;
            }

            .small {
                width: 38px;
            }
        }
    }
}
</style>