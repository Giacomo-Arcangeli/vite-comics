<script>
export default {
    data() {
        return {
            links: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'News',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false,
                },
            ]
        }
    }
}
</script>


<template>
    <header class="container">
        <img src="../assets/img/dc-logo.png" alt="">
        <nav>
            <ul>
                <li v-for="link in links" :key="link.text">
                    <a :href="link.url">{{ link.text }}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>


<style lang="scss" scoped>
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 140px;
}

img {
    max-width: 80px;
}

ul {
    display: flex;
}

li {
    margin: 0 12px;
    text-transform: uppercase;
    font-weight: 700;

    &:hover {
        color: rgb(2, 130, 249);
        text-decoration: underline;

        a {
            color: rgb(2, 130, 249);
        }
    }

}
</style>