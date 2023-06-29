<script>
export default {
    data() {
        return
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
        ];
    }
}
</script>


<template>
    <header>
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
    height: 120px;
    border: 2px dashed red;
}

img {
    max-width: 80px;
    margin-left: 10px;
}

ul {
    display: flex;
}

li {
    margin: 0 12px;

    &:hover {
        color: rgb(2, 130, 249);
        border-bottom: 5px solid rgb(2, 130, 249);
    }
}
</style>