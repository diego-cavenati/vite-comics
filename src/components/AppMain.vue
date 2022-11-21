<script>
import HeroImage from './HeroImage.vue'
import Banner from './Banner.vue';
import ComicsList from './ComicsList.vue';

export default {
    name: 'AppMain',
    components: {
        Banner,
        ComicsList,
    },
}
</script>

<template>
    <main>
        <HeroImage />
        <ComicsList />
        <Banner />
    </main>
</template>

<style lang="scss" scoped>

</style>