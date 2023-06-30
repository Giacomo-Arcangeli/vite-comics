<script>
import ComicCard from './ComicCard.vue';
export default {
    components: { ComicCard },
    props: {
        comics: Array
    }
};
</script>

<template>
    <main>
        <figure></figure>
        <!-- top -->
        <section class="section-top">
            <div class="container">
                <h2 class="series">CURRENT SERIES</h2>
            </div>
            <div class="card-container container">
                <ComicCard v-for="comic in comics" :key="comic.series" :comic="comic" />
            </div>
            <div class="container center">
                <h3 class="load">LOAD MORE</h3>
            </div>

        </section>

        <!-- bottom -->
        <section class="section-bottom">
            <ul class="container center">
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
figure {
    background-image: url(../assets/img/jumbotron.jpg);
    height: 400px;
}

.container {
    position: relative;
}

.series {
    color: white;
    padding: 10px 15px;
    border: 2px solid rgb(2, 130, 249);
    background-color: rgb(2, 130, 249);
    position: relative;
    bottom: 28px;
    font-weight: 600;
}

.section-top {
    color: white;
    background-color: rgb(28, 28, 28);
    min-height: 140px;

    div {
        display: flex;
        align-items: center;
        height: 100%;
    }
}

// card
.card-container {
    display: flex;
    flex-wrap: wrap;
    padding: 50px 0;
}

.card {
    flex-basis: calc(100% / 6);
}

.center {
    display: flex;
    justify-content: center;
}

.load {
    color: white;
    padding: 10px 50px;
    border: 2px solid rgb(2, 130, 249);
    background-color: rgb(2, 130, 249);
    cursor: pointer;
    margin-bottom: 20px;
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