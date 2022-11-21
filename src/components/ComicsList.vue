<script>
import ComicCard from './ComicCard.vue';
import comics from '../data/comics.js';


export default {
    name: 'ComicsList',
    component: {
        ComicCard,
    },
    data() {
        return {
            comics,
        }
    }
}
</script>
<template>
    <section class="comics">
        <h2>Current Series</h2>
        <div class="container">
            <div class="row">
                <ComicCard v-for="comic in comics" :thumb="comic.thumb" :series="comic.series" />
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables.scss' as *;

.comics {
    h2 {
        background-color: $dc-primary;
        display: inline-block;
        padding: 0.5rem 1rem;
        margin-top: -2rem;
        margin-bottom: 3rem;
    }
}
</style>