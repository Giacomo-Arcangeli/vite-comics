<script>
export default {
    props: {
        comic: Object
    }
}
</script>

<template>
    <div class="card">
        <img class="comic-fig" :src="comic.thumb" :alt="comic.series">
        <h4>{{ comic.series }}</h4>
    </div>
</template>

<style scoped>
.card {
    display: flex;
    flex-direction: column;
}

.comic-fig {
    width: 200px;
    height: 230px;
}

h4 {
    text-align: center;
    padding: 20px;
    margin-bottom: 40px;
}
</style>