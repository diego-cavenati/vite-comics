<script>
export default {
    name: 'ComicCard',
    props: {
        thumb: String,
        series: String
    }
}
</script>
<template>
    <div class="col">
        <div class="comic">
            <img :src="thumb" :alt="series">
            <h3>{{ series }}</h3>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.comic {
    width: 100%;

    img {
        max-width: 100%;
    }
}
</style>
