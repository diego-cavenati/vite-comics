<script>
import ComicCard from './ComicCard.vue'
import comics from '../data/comics.js'
export default {
    name: 'ComicsList',
    components: {
        ComicCard
    },
    data() {
        return {
            comics
        }
    }
}
</script>

<template>
    <section class="comicsList">
        <div class="container">
            <h2>Current Series</h2>
            <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 row-cols-lg-6">
                <ComicCard v-for="comic in comics" :thumb="comic.thumb" :series="comic.series" />
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

.comicsList {

    h2 {
        display: inline-block;
        padding: 0.5rem 1.5rem;
        background-color: $dc-primary;
        margin-top: -2rem;
        margin-bottom: 4rem;
    }

    padding-bottom: 3rem;
}
</style>